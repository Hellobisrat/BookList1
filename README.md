
# content provider

this project mainly covered
about content provider and reducer
using createcontext and useReducer 
hooks

# example of creating context
const BookContext = createContext();

# lets see how create contextProvider 

export const ThemeContext = createContext();

const ThemeContextProvider extends Component {
  state ={
    isLightTheme: true,
    light: { syntax: '#555', ui:'#ddd', bg:'#eee'}
    dark: { syntax:'#ddd', ui:'#333', bg:'#555'}
  }
}
render(){
  return
  <ThemeContext.Provider value={{...this.state,toggleTheme}}>
  {this.props.children}
  </ThemeContext.Provider>
}

# it has also context provider in functional form

# August 27 2024

# Bisrat Mengesha

# Dallas Tx
