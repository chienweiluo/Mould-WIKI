## **Q: What's the difference between Mould and  the traditional UI builder using drag-and-drop ?**

After a simple analysis, we distinguished the functional differences between **Mould** and other tools, **VB** and **Storyboard**


### **VB**

**VB** represents this kind of tool: 
>  *Developer redevelops the generated GUI code from the tool.*

The generated code is unable to be imported into the tool for secondary design process, which means that the maintenance of the UI still depends on the developer's handwriting.

**Mould** will completely separate the GUI and the program. You can modify the GUI at any time without worrying about unexpected problems in the program.

### **Storyboard**

The first thing to say is that  the author of **Mould** hasn’t engaged in iOS development, but only briefly studied the API.

Storyboard is based on classic MVC. A man can achieve dynamic data interaction by operating the View widget in the Controller.

The tool is hard to achieve high-fidelity. It will cause a situation that the UI will be completely different from the composed components in the editor when program runs. Simply put, the tool has limited control over UI.

In contrast, **Mould** achieves high fidelity when editing, ensuring the UI in editor can accurately appear in the running program.And whole interaction and visual in UI and are predictable.


It is noteworthy that the SwiftUI Apple launched in 2019 follows the the design paradigm of React. It does not provide a editing tool itself. Which means that Apple wants to overthrow the way, Storyboard as a GUI maker, created by themselves. 


As for another technology giant, Google also launched Jetpack Compose at about the same time, which is also the design paradigm of React. 

Back to **Mould**, **Mould** is a higher-level framework of the React paradigm, perfectly retaining the efficiency and power of React.

<br/>

## **Q: How to achieve cross-end ?**

**Mould** is only focus on GUI building. The approach **Mould** achieve cross-end is like GraphQL. Each end has its own runtime, which excute the Schema following **Mould**. Therefore, each end can use its own lang(or ecology), and the uniqueness of each end is also preserved.

Compared to Flutter, **Mould** not only can achieve a high consistency at each end of GUI, but also can smoothly integrate the App on each end to become part of the existing project.

<br/>

## **Q: What is the advantage that does the drag-n-drop tool is better than the handwritten in efficiency？**

- Reduce difficulty
- More User-friendly.
- Adjust stepless.
- Immediate feedback

<br/>

## **Q: Is there any flexibility limit? Can Mould generate complex applications beyond simple static pages ?**

In comparison with traditional tool for page building, **Mould** is more flexible without giving up anything about flexibility. Its power is consistent with React.What React can do, **Mould** also can do.

Noteworthy, **Mould** is implemented using React. So, **Mould** is able to do self-bootstrapping.

<br/>

## **Q: How to transform designers' work into a running interface？**

Regardless of the design tools (Figma and Sketch), the files they export can be regarded as groups of vector Config and non-vector Binary Assets.

**Mould** is the same.

<br/>

## **Q: Is there a lack of expressiveness on design ?**

Currently, the editor of **Mould** is based on DOM, and its power is rely on the expressive power of DOM as the infrastructure of GUI.
And because the UI that **Mould** equipped now only runs on the DOM, **Mould** can be self-sufficient.


In the future, as more ends are handled, we may find a way between the intersection and union of expressive forces at each end. At present, we prefer take union, so that expression power of **Mould** may be "overflowed" rather than missing relative to a single end. Graceful downgrade would be a good idea to solve the "overflow" problem.

<br/>

## **Q: How the exported result through design fulfil the requirements of App ? Does it increase the difficulty of the designers' work ?**
Answer this Q from the following 3 dimensions.
- Style.
- Layout.
- Robustness.

#### Style

Style is the easiest part to transform from design to application. As for adjusting the parameters on the design panel, **Mould** is the same as the traditional design tool.

#### Layout

First, with the outbreak of smart devices,Responsive is more and more important in applications and design.

In order to run the UI directly, its adaptive ability (responsive) must be considered in the design process.

**Mould** provides an responsive Stack layout, which requires designer to use it for design on responsive component. This way has already paved by another pioneer.But it is relatively new, so it is necessary to explore and combine practice in real development.

#### Robustness

The designer's current work flow ends with "eye check", which means that as long as the final designed interface is beautiful to meet their own thought, the work is done.But the applications need to increase usability and robustness considerations.

For example, a front-end engineer received an "expression" image for a paragraph of text that the length of the paragraph does not matter, just look good. However, the paragraph runs in real world may be many situations need to concerned, e.g. too long or too short, break the line, display ellipsis in trucated part , and so on.
As for this part of information, it would not be shown in the design draft. And the one of the important point **Mould** want to carry out is that the designer is fully responsible for the entire visual interaction effect in handling design process.

### **Conclusion**

It seems that designers' job go much harder, but let us think about the current scenario, 

> how to make a set of layout Responsive ?

Actually, the engineer need to communicate with the designer.If they have not considered this point in design process, they need to have an answer at once. And if the current design is too hard to implement, the work need to back to design and revise repeatedly. The same is for the issue of robustness.

**Mould** clarify these factors that originally need to be considered by designer.(Responsive), or directly return back the responsibility and the ability to implement to the designer (design shipped to  production directly)

**Mould** let designers and engineers autonomy in their own work, that means designer and engineer will work together but in parallel.

**Mould** achieve the unification of responsibility and ability

**Mould** greatly reduce the cost of communication. Instead of increasing the GUI design chore, **Mould** only clarifies what should be done in the design process.
