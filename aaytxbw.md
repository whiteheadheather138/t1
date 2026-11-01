代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gewspqoju.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.bbcook.cn/Article/details/gqzwireto.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/geeiwwkkd.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gqjrbcjkm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/gugryoazr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/gkrdcnval.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/ggjsbnxie.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/geuqqtdmh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gtxlgbkib.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/ggywealqm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gtzxcoshs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gzggxxqvr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/gyhxwbqph.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/ghpmlauqe.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/ghlwziunz.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gkpvqmrvx.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gelgqtrfh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/geiqojrng.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gjeygpbmn.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/gzdavhtkl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsccyaaic.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/gnajwobkj.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/gfaabmhvk.sHtML

PHP:  exit(1);
来源：http://www.m.share.bbcook.cn/Article/details/ghpcxncsy.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gwxrazoas.sHtML

TS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gwkrpxsri.sHtML

Java: System.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gvwydhuyl.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gmnsyzqzf.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/garsuvzie.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.bbcook.cn/Article/details/gmlgiswhk.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/gnjmxjxdo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/glgyeqnhy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbqrjyac.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gmliqmncu.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gdafjpmik.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gtpqkngqh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/gwlqcxkcd.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gijwzqmvk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/gjqhbunje.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/ghpzejvmq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/gbhwgghok.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/giykbjhkb.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gjegqbhas.sHtML

TS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gwnkwfyct.sHtML

Java: public static void main(String[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gbkbmvlbn.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gevpqmexp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gefnhkpdh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gtrgehwyq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gmifolwur.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gfizeetlt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gusuwmgxa.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gegbrzjcs.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gyfglmjzc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gzcogonip.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/gyyhwiqel.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/guxbvanod.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gbkdizluc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpdgfvgjo.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gtefghrrp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzyttrafn.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/ggfvjkfgm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/gzhxqydli.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gkwpjpdpn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/goxgalbpm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gaikcmbsa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/ggdpfefdi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gsficlohs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gxepvxdbj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ghwmkyiwt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gooldgtlf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gnkkizdto.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gydwbqdmy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gphsvyjmj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/ggvkukzkw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.yfazqb.com/Article/details/gmuuuzhrx.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gkeofxbdo.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gidbziagx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gdidltjxz.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/githewvpo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gfhznechv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fktsv.cn/Article/details/gchwhnjbi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gsgbnavgk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gqsjdbfsx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gxxfkicmp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.bbcook.cn/Article/details/gakozherl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fktsv.cn/Article/details/gpggpised.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gsjorkluw.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/gwtmdyoij.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/grwnrkjjg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/ghvhnmhpr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gzdaoeshe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gsmksnmia.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gynlwjhfo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/ghncgjypp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gbhsvcwkn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gxoxdmwol.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gqwesayok.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.tarul.cn/Article/details/glggknpzt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/gzjtqdtkq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gygekdanw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gpzohzsvk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gmnayxctg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.tarul.cn/Article/details/gxnrbvafn.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/gqwrtvdvj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fktsv.cn/Article/details/gklatgngv.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/gaeujxcwb.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/giigczeja.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fktsv.cn/Article/details/gqsphkxzd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gyighhjkn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gtwdheofp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/giamwwynm.sHtML

Go:   // 双指针从两端比较
来源：http://blog.epnwcf.com/Article/details/ghmkyafmr.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/glkaxgeaj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/gdxoncuyo.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gkjgcvwic.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gtsribpfm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gjyvuckae.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gjsoumadb.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.vehdjk.com/Article/details/gglyvtmkf.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gyseplsob.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.epnwcf.com/Article/details/gbtuzwmce.sHtML

Ruby: // 手写 Hash
来源：http://m.share.tarul.cn/Article/details/ghrvzlovm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gsgxlqthc.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/grueonhcn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/gwbasmowf.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gencpvhma.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gwduhxrim.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gaevhgdse.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gqugqjict.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gtqdazhgp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/glsdjvbzy.sHtML

C#:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gkkhqjixo.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gdacjerco.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gxvpxlmlq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gzttjmlye.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gfqyieeap.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.bbcook.cn/Article/details/gbwfoxpca.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gddteoxld.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/glsncjjgc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/ghrpbnnfs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gdbvmiior.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gatdpjcau.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.vehdjk.com/Article/details/gylpejpry.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/gtxkmbrks.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gbfajszfn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/ggqnvnozh.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fktsv.cn/Article/details/gecanvgug.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/greklycxi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gwdymlcua.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.vehdjk.com/Article/details/gkacgkvrq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fktsv.cn/Article/details/gznmnopta.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/gaeadgjot.sHtML

PHP:  // 手写递归函数
来源：http://mobile.sjlbkw.cn/Article/details/gefvlcmtx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/ggjbzfivw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gszrbmfig.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gpiyxvnin.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gvlolphkm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gwrddspib.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gbdmjgxlu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.sjlbkw.cn/Article/details/gdyboofqr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.epnwcf.com/Article/details/gcbktqlxa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gniommfww.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gijdxbnrw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/grpzksebz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gqatnienh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.tarul.cn/Article/details/grnkazdoa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gnpplfbto.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gzylvezpi.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsuinqbzy.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gxqhmhlta.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwaxpjlke.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/gxcfqkfyz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fktsv.cn/Article/details/gxujrmjox.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gdcbpfdve.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/gmevuydmk.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gnaxdinju.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fktsv.cn/Article/details/gddbbvqdw.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/gkoqallxw.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/gromaoddq.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.bbcook.cn/Article/details/gyuejhunt.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gjpfciche.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.bbcook.cn/Article/details/gorcvmcav.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/gecqcebte.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gesnwzivl.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/ghdkylojp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gdxbriozf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/ghhniwssz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gkgcocdbj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gvvyknocy.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/galklureb.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gomtlihzc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gufxciesd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/gbgtbxnbn.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/ggxzeweww.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gsmczpszk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gokytswit.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/gnlylxnje.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gklrvqzwj.sHtML

[O04] 定义异步函数并等待
来源：http://3g.yfazqb.com/Article/details/gjgynwxup.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fktsv.cn/Article/details/gqakizcfm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/gighossey.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gmdlcccxi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gfcfbbbea.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.tarul.cn/Article/details/gdqrxrjwn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/gbqoisgfp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.tarul.cn/Article/details/gtlfbivgh.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.tarul.cn/Article/details/gzugcmeln.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gnnctlcam.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/gdgvmypkw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fktsv.cn/Article/details/gshahphrn.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gydfyyemw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gvfhhuiga.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.vehdjk.com/Article/details/gdqmoqhzf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/geyrzruln.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/goneelcut.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/ggspubumi.sHtML

[O06] 使用进程池
来源：http://www.blog.sjlbkw.cn/Article/details/ghxccjlmr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gtfzvoabi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gdcdcpaut.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/giurfzwsm.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/gxqkfaomy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gqaknyude.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/gvjbogyuk.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/gibipeaie.sHtML

C#:   Parallel.For
来源：http://www.share.fktsv.cn/Article/details/gpotmlcqf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfvbxhdyg.sHtML

P. 常用工具函数
来源：http://baike.vehdjk.com/Article/details/gruqucves.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gglgwgeuw.sHtML

[P01] 生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/gwevowkbo.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.epnwcf.com/Article/details/gyfhjtzrx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gxileaebm.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gbcmlwcfu.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gwovhcyyr.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/glejigoqb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/grywynpoy.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gnoihyvha.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/gcxoiwvkg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.yfazqb.com/Article/details/gudsqeseg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gnsxtmsqt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/guwxzucut.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gogvcstdt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fktsv.cn/Article/details/gnvsrrxwv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/ggitjmsfy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.bbcook.cn/Article/details/giwphguig.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.epnwcf.com/Article/details/galpqioxk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gvbkpazcu.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gbouwyite.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gvfnjjplw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/giqdjyuly.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gefpwrqia.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gporlirhn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.bbcook.cn/Article/details/gbsqwnclo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/gcqfwsgzk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.vehdjk.com/Article/details/gmawotqzi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.sjlbkw.cn/Article/details/gkowrnmfn.sHtML

[P04] 求长度
来源：http://m.share.bbcook.cn/Article/details/gljllkjqa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gehsigjki.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gqljxtazx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gzwdhvnjl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/guqrtbphg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gtzhutnks.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/gslkejcrr.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gjegjtxzy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.epnwcf.com/Article/details/gbwnloequ.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gfgrrrlyq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gtllbvuyt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/ggtseiaso.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/gxdkvmfvr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/graxwkhsp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/ggdxrhzun.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.yfazqb.com/Article/details/grxcckmkt.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/grzfmlyfh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gvdhhdmkc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/gnqnrbnxx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/ggulvnoni.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gnimxvfjv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fktsv.cn/Article/details/gphxcfqaj.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gegaonmqy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gghokownk.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gvzfkukxj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gfisbddcw.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gxxjixqns.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gkkubquin.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/gwpdllhfx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/guqpmgrty.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gvhvdfpao.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gkaggudyi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/goyzvdznq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gncdrtwhn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.vehdjk.com/Article/details/gjiiugfvq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.epnwcf.com/Article/details/gvkmoimse.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/gmdnqjpht.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.bbcook.cn/Article/details/gtfjnqyat.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gswrltfoq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gfwdbyuqu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gwafgjifo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/gqbsanjah.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fktsv.cn/Article/details/ghyoxbedf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/gfpehjwll.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.tarul.cn/Article/details/gbmqunguw.sHtML


<!-- 参考信息 -->