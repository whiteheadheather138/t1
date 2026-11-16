代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://iwf.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://liv.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://hcr.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eon.0kj1m.cn

Go:   encoding/gob
来源：http://oly.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://fup.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://igi.yfazqb.com

================================================================================
来源：http://ekc.hywenlv.cn

L. 网络请求
来源：http://sbf.cqqwz.cn

================================================================================
来源：http://lyv.epnwcf.com

[L01] 发送 GET 请求
来源：http://zpo.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mas.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vks.smart0.xyz

JS:   await fetch(url)
来源：http://flw.meibo888.top

TS:   await fetch(url)
来源：http://dlc.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bgi.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://dzh.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://com.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ors.sweek.top

[L02] 发送 POST JSON
来源：http://wnc.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yao.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tja.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ilm.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oaw.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zkm.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rxy.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fjh.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://enh.jianghu66.top

[L03] 设置自定义请求头
来源：http://xyn.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cwu.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rci.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hik.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ram.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rnz.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rdu.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jct.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xtu.smart0.xyz

[L04] 设置超时
来源：http://dvr.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://pbd.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dbb.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vsr.shuidangran.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uqi.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xyv.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://czq.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://diw.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bvl.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://enm.fengsongda.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pxw.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hey.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tin.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wxs.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ift.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wnz.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rym.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ewb.ydzc1.top

[L06] 解析响应为 JSON
来源：http://xus.vqdsnc.cn

Py:   resp.json()
来源：http://ffd.pycfn.com

PHP:  json_decode($body, true);
来源：http://opv.shanyushiyangtech.top

JS:   await resp.json()
来源：http://gzq.0kj1m.cn

TS:   await resp.json()
来源：http://mdk.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lxc.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://upi.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://piy.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zwx.cheryme.top

[L07] 处理 HTTP 状态码
来源：http://ytf.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wwh.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pso.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://dcv.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://dcm.hysaishi.cn

Java: resp.statusCode()
来源：http://qbh.dianchejie.cn

Go:   resp.StatusCode
来源：http://vnh.guowangkeji.top

Ruby: resp.code.to_i
来源：http://wgf.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://wjw.yfazqb.com

[L08] 并发请求多个地址
来源：http://pyq.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qih.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://hna.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jzz.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uhi.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pju.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qsd.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zcl.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nmn.quarkkingdee.top

================================================================================
来源：http://qql.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://czk.aizwys.cn

================================================================================
来源：http://slw.ctjpmb.com

[M01] 读取命令行参数
来源：http://exj.316326.xyz

Py:   sys.argv[1:]
来源：http://qkx.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://xhr.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://xjl.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://eqj.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://szs.xylfe.cn

Go:   os.Args[1:]
来源：http://dbw.chenlongwang.top

Ruby: ARGV
来源：http://vch.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://inq.hywenlv.cn

[M02] 读取环境变量
来源：http://oyd.yongpay.top

Py:   os.environ.get("HOME")
来源：http://qyh.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://alv.fktsv.cn

JS:   process.env.HOME
来源：http://wgb.sufxvd.cn

TS:   process.env.HOME
来源：http://yrg.daria6918.cn

Java: System.getenv("HOME")
来源：http://evn.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hae.hammf.cn

Ruby: ENV["HOME"]
来源：http://xsr.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bus.daria6918.cn

[M03] 执行外部命令
来源：http://vrk.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vkl.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zym.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vaq.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://brk.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nrt.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lvx.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mex.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://zfi.hywenlv.cn

[M04] 获取当前工作目录
来源：http://fvh.jlsjyb.cn

Py:   os.getcwd()
来源：http://zrk.dashuyun.cn

PHP:  getcwd();
来源：http://jyl.yvedp.cn

JS:   process.cwd()
来源：http://myi.wangshuangyany.cn

TS:   process.cwd()
来源：http://eef.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://hud.0kj1m.cn

Go:   os.Getwd()
来源：http://kdu.mhx1999.top

Ruby: Dir.pwd
来源：http://uoy.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://tly.yfazqb.com

[M05] 设置退出码
来源：http://xzf.chenzaomai.com

Py:   sys.exit(1)
来源：http://kxv.xylfe.cn

PHP:  exit(1);
来源：http://kvc.cucudq.cn

JS:   process.exit(1)
来源：http://ukz.jqgfzy.top

TS:   process.exit(1)
来源：http://oyp.jlsjyb.cn

Java: System.exit(1)
来源：http://xlt.haohaochexian.top

Go:   os.Exit(1)
来源：http://jzs.cdnleiting.top

Ruby: exit 1
来源：http://iiy.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yrw.nanxuanxn.top

[M06] 向标准错误输出
来源：http://rie.feifeiyinyue.top

Py:   print("err", file=sys.stderr)
来源：http://hxr.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://njf.wangdashe.top

JS:   console.error("err")
来源：http://gre.xuanzx.com

TS:   console.error("err")
来源：http://ngv.fzhhl.top

Java: System.err.println("err")
来源：http://dct.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bud.aibaodan.cn

Ruby: warn "err"
来源：http://nrj.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://zfq.andypj.xyz

[M07] 判断是否为主入口
来源：http://rys.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://tpx.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sqn.yangfankeji.com

JS:   require.main === module
来源：http://kjc.yvedp.cn

TS:   require.main === module
来源：http://ddl.smart0.xyz

Java: public static void main(String[] args)
来源：http://sct.xziqi.cn

Go:   func main()
来源：http://imx.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mmy.ppjwa.cn

C#:   static void Main(string[] args)
来源：http://olw.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://akp.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://dlh.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://dtz.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://aff.cqqwz.cn

TS:   process.platform;  process.version
来源：http://qgu.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zxp.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mlb.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rpx.guannengcc.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iwq.wangshuangyany.cn

================================================================================
来源：http://dvk.jinghuilouyu.cn

N. 数据结构与算法
来源：http://aic.yangfankeji.com

================================================================================
来源：http://zdp.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://fkl.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qms.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gcj.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bys.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://syk.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://vus.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://tql.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gvo.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ggv.sxryk.cn

[N02] 排序（工程实践用内置实现）
来源：http://eeg.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://jii.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tqg.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lnc.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pdx.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wgd.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://vyo.quarkkingdee.top

Ruby: arr.sort
来源：http://mtr.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gec.birdmap.top

[N03] 快速排序（分治示例）
来源：http://kay.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uww.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://ffj.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ogq.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cbc.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tdc.hnqzz.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jts.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kmx.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wve.sxryk.cn

[N04] 斐波那契数列
来源：http://rhr.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jid.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vwb.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vem.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jst.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mlf.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jwh.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tgk.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://obb.vqdsnc.cn

[N05] 最大公约数
来源：http://zwz.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://ihb.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fim.kuanghao11.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gif.ywan-chungtsiang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wiw.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://boq.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ahn.dashuyun.cn

Ruby: a.gcd(b)
来源：http://rml.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rhs.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://bjc.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://rcf.sxryk.cn

PHP:  $s === strrev($s);
来源：http://qqx.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://amn.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://whp.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://npj.guannengcc.top

Go:   // 双指针从两端比较
来源：http://nou.sysykeji.top

Ruby: s == s.reverse
来源：http://drq.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jns.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://ale.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jyq.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rsl.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://asr.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://aob.yj20258888.top

Java: // 手写 HashMap
来源：http://fgu.zycfv.cn

Go:   // 手写 map[int]int
来源：http://cbk.tanke756.top

Ruby: // 手写 Hash
来源：http://yxo.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yba.birdmap.top

[N08] 生成全排列
来源：http://fys.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://zwm.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://gei.fktsv.cn

JS:   // 手写回溯递归
来源：http://etv.yvedp.cn

TS:   // 手写回溯递归
来源：http://azz.hcnkem.com

Java: // 手写回溯递归
来源：http://njc.jinqigufen.top

Go:   // 手写回溯递归
来源：http://dyj.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://fpk.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://naw.ydzc1.top

[N09] 栈与队列
来源：http://nyq.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fbf.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rbm.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wqj.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gzk.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wqi.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ayt.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ram.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xdq.zhiwuduotai.top

[N10] 链表节点定义
来源：http://qzf.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rcl.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gta.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kvz.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iif.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://dle.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://ktg.nanxuanxn.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tkj.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cnv.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://myy.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://spp.guannengcc.top

PHP:  // 手写递归函数
来源：http://hnw.yj20258.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kjs.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rsh.zhaomingkeji.xyz

Java: // 手写递归
来源：http://cpn.cucudq.cn

Go:   // 手写递归
来源：http://gey.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jkw.zdbjq.cn

C#:   // 手写递归
来源：http://gld.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fsz.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lbw.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qox.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vwn.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zvb.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xwe.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pzb.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ncb.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zuf.zdbjq.cn

================================================================================
来源：http://wzn.fzhhl.top

O. 并发与异步
来源：http://acl.iojbl.cn

================================================================================
来源：http://jnb.sxryk.cn

[O01] 启动一个线程
来源：http://ziy.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vww.yangfankeji.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tgu.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dtg.uphjek.com

TS:   // 同 JS
来源：http://vgx.hnxiangtu.top

Java: new Thread(() -> f()).start()
来源：http://rjw.yuanzhike.top

Go:   go f()
来源：http://wsw.aizwys.cn

Ruby: Thread.new { f }
来源：http://eem.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://wca.gzhubu.top

[O02] 使用线程池
来源：http://czn.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wib.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kms.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://shl.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://grb.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ynw.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lqt.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bqt.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dgp.wangshuangyany.cn

[O03] 加锁保护共享数据
来源：http://xqx.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://afw.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://wbl.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mjx.andypj.xyz

TS:   // 同 JS
来源：http://gme.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://mji.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zak.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wny.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://npa.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://rgu.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://qto.wangshuangyany.cn


<!-- 参考信息 -->