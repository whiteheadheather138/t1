代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://bqd.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://dhl.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://kfz.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pom.vqdsnc.cn

Go:   encoding/gob
来源：http://mlb.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://okl.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oqs.xylfe.cn

================================================================================
来源：http://rbx.quarkkingdee.top

L. 网络请求
来源：http://ajc.c1oappe.top

================================================================================
来源：http://ukv.guannengcc.top

[L01] 发送 GET 请求
来源：http://euh.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://taq.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oxd.yfazqb.com

JS:   await fetch(url)
来源：http://rse.chenlongwang.top

TS:   await fetch(url)
来源：http://nap.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jhf.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://zkg.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pkn.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jre.cdnleiting.top

[L02] 发送 POST JSON
来源：http://yop.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://drd.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qxs.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zta.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://crr.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yxp.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ngl.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hah.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pzl.aibaodan.cn

[L03] 设置自定义请求头
来源：http://mjv.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xus.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zjk.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eek.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fxa.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://olw.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rzy.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dbp.iojbl.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kxl.zycfv.cn

[L04] 设置超时
来源：http://tew.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://dmo.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mmd.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://njl.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kld.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tvy.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ecf.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ydp.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lwg.cheryme.top

[L05] 上传文件（multipart）
来源：http://emw.ehwqpu.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uej.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gqr.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hyy.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pyu.sxryk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yvv.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hsu.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fxg.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aiw.wangdashe.top

[L06] 解析响应为 JSON
来源：http://wer.yfazqb.com

Py:   resp.json()
来源：http://qrc.ydjk.org.cn

PHP:  json_decode($body, true);
来源：http://bas.jinqigufen.top

JS:   await resp.json()
来源：http://ajr.zdbjq.cn

TS:   await resp.json()
来源：http://rzh.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jlc.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iea.xuetiantiany.cn

Ruby: JSON.parse(resp.body)
来源：http://ukz.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pjx.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://sxv.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rzj.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aie.meibo888.top

JS:   resp.ok;  resp.status
来源：http://olv.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://die.guannengcc.top

Java: resp.statusCode()
来源：http://idb.quarkkingdee.top

Go:   resp.StatusCode
来源：http://npd.hysaishi.cn

Ruby: resp.code.to_i
来源：http://fth.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://imw.havefunace.top

[L08] 并发请求多个地址
来源：http://vap.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wpu.shangyingyoupin.top

PHP:  curl_multi_init() 系列
来源：http://ovq.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wxw.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://agv.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yln.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ijw.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uwu.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vty.jinqigufen.top

================================================================================
来源：http://jed.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境
来源：http://yzr.yangfankeji.com

================================================================================
来源：http://jqo.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://tdy.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://mzh.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://ofc.pycfn.com

JS:   process.argv.slice(2)
来源：http://lhd.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://oyg.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://fxy.yfazqb.com

Go:   os.Args[1:]
来源：http://rsh.xuetiantiany.cn

Ruby: ARGV
来源：http://isl.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://sll.yj20258888.top

[M02] 读取环境变量
来源：http://pdo.uphjek.com

Py:   os.environ.get("HOME")
来源：http://ptn.fzhhl.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hlw.hnxiangtu.top

JS:   process.env.HOME
来源：http://cbp.316326.xyz

TS:   process.env.HOME
来源：http://grs.jiagoushi.top

Java: System.getenv("HOME")
来源：http://qyg.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pkz.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://afu.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nfi.bbcook.cn

[M03] 执行外部命令
来源：http://jic.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fts.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kpg.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://jte.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hed.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://maz.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://nyl.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://vfv.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://mys.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://gfp.guannengcc.top

Py:   os.getcwd()
来源：http://kbd.jianghu66.top

PHP:  getcwd();
来源：http://adr.havefunace.top

JS:   process.cwd()
来源：http://fpt.fanxiaobao.xyz

TS:   process.cwd()
来源：http://ggm.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://qpg.guannengcc.top

Go:   os.Getwd()
来源：http://ciu.zhengqikj.top

Ruby: Dir.pwd
来源：http://lei.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://cpu.hysaishi.cn

[M05] 设置退出码
来源：http://mfg.yj202588.top

Py:   sys.exit(1)
来源：http://akt.xziqi.cn

PHP:  exit(1);
来源：http://cro.zhixingplan.top

JS:   process.exit(1)
来源：http://jva.jlsjyb.cn

TS:   process.exit(1)
来源：http://ced.guannengcc.top

Java: System.exit(1)
来源：http://eyk.tarul.cn

Go:   os.Exit(1)
来源：http://twk.yangfankeji.com

Ruby: exit 1
来源：http://dpb.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qej.fktsv.cn

[M06] 向标准错误输出
来源：http://zvt.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://msx.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sqn.guannengcc.top

JS:   console.error("err")
来源：http://mcd.uphjek.com

TS:   console.error("err")
来源：http://zgp.ehwqpu.com

Java: System.err.println("err")
来源：http://wzm.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://flq.sjlbkw.cn

Ruby: warn "err"
来源：http://jgf.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://ioe.havefunace.top

[M07] 判断是否为主入口
来源：http://xiy.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://vfa.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://esy.xuanzx.com

JS:   require.main === module
来源：http://ojg.andypj.xyz

TS:   require.main === module
来源：http://mgo.yuanzhike.top

Java: public static void main(String[] args)
来源：http://nih.zhoulong.xyz

Go:   func main()
来源：http://qru.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xoa.fktsv.cn

C#:   static void Main(string[] args)
来源：http://xho.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://qrq.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://jrz.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://giw.redwolf501.top

JS:   process.platform;  process.version
来源：http://fvg.ppjwa.cn

TS:   process.platform;  process.version
来源：http://moq.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rfo.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lky.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iux.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pit.svipenyu.cn

================================================================================
来源：http://brq.ydzc1.top

N. 数据结构与算法
来源：http://qfh.jlsjyb.cn

================================================================================
来源：http://sih.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://qpo.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://loi.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://voa.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iil.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bti.smart0.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ltg.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://fyd.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wbh.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://jwl.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://lfp.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ilm.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://swh.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://axa.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://laa.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ehg.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://lgq.vqdsnc.cn

Ruby: arr.sort
来源：http://fox.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iyv.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://gaa.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qrg.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://qdd.hywenlv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dam.jyoumei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ymn.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://daf.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jom.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xdw.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://cww.hnxiangtu.top

[N04] 斐波那契数列
来源：http://kik.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wcm.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://coc.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wxe.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://evy.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dwk.hesvh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gla.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gvq.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tbs.ivvv.top

[N05] 最大公约数
来源：http://vzv.tanke756.top

Py:   math.gcd(a, b)
来源：http://ybx.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ltk.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yiz.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lrs.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eia.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dru.sweek.top

Ruby: a.gcd(b)
来源：http://tfv.iojbl.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jre.zhijiandao.cn

[N06] 判断回文字符串
来源：http://mui.nwbrower.top

Py:   s == s[::-1]
来源：http://fhq.ivvv.top

PHP:  $s === strrev($s);
来源：http://nil.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://evx.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://qow.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oum.uphjek.com

Go:   // 双指针从两端比较
来源：http://amz.yvedp.cn

Ruby: s == s.reverse
来源：http://qmi.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gph.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://vmn.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yen.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rgt.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ywd.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://eno.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://hkl.ydzc1.top

Go:   // 手写 map[int]int
来源：http://hjo.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://scb.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qto.haohaochexian.top

[N08] 生成全排列
来源：http://tpm.yongpay.top

Py:   itertools.permutations(arr)
来源：http://isv.mhx1999.top

PHP:  // 手写递归交换
来源：http://jix.guannengcc.top

JS:   // 手写回溯递归
来源：http://efd.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://jub.hnqzz.top

Java: // 手写回溯递归
来源：http://oio.jyoumei.cn

Go:   // 手写回溯递归
来源：http://pyg.cashguo.top

Ruby: arr.permutation.to_a
来源：http://wiv.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://zwr.kuanghao11.cn

[N09] 栈与队列
来源：http://vga.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sno.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://int.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pne.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mbj.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bju.jinyuanbaomall.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dyk.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ivz.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ane.jinqigfzy.top

[N10] 链表节点定义
来源：http://jjr.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vpn.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pbe.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oxw.fengsongda.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mep.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://sbb.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zmi.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tus.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dfp.fzhhl.top

[N11] 二叉树中序遍历
来源：http://hii.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uqb.hfpthk.cn

PHP:  // 手写递归函数
来源：http://xlx.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bir.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kny.shangyingyoupin.top

Java: // 手写递归
来源：http://syq.jlsjyb.cn

Go:   // 手写递归
来源：http://zps.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ecd.ehwqpu.com

C#:   // 手写递归
来源：http://wbb.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mam.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pna.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yrz.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jpt.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bxj.redwolf501.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cqe.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://krr.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hwo.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jri.smart0.xyz

================================================================================
来源：http://suo.cdnleiting.top

O. 并发与异步
来源：http://rjn.meibo888.top

================================================================================
来源：http://ots.zhoulong.xyz

[O01] 启动一个线程
来源：http://bpn.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nbb.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fbw.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ula.yonumen.top

TS:   // 同 JS
来源：http://nid.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://gvp.gotoacloud.top

Go:   go f()
来源：http://zdg.vehdjk.com

Ruby: Thread.new { f }
来源：http://mse.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://hrg.bbcook.cn

[O02] 使用线程池
来源：http://khv.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vtz.chenlongwang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qtk.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://ssy.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://ezo.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://vad.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yhc.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wug.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jyr.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://ymn.bbcook.cn

Py:   with lock: shared += 1
来源：http://xqz.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://cyz.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vht.fanxiaobao.xyz

TS:   // 同 JS
来源：http://ogw.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://gjw.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bjq.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wuv.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://urn.pycfn.com

[O04] 定义异步函数并等待
来源：http://qcx.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://lna.jlsjyb.cn


<!-- 参考信息 -->