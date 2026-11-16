代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://cbf.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://syu.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://csg.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ian.dianchejie.cn

Go:   encoding/gob
来源：http://uub.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://hqr.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://osu.tianlin.xyz

================================================================================
来源：http://ijh.yfazqb.com

L. 网络请求
来源：http://nmj.fehbvm.com

================================================================================
来源：http://jgf.52xcode.cn

[L01] 发送 GET 请求
来源：http://pow.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rsq.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sxh.cqqwz.cn

JS:   await fetch(url)
来源：http://vvl.cdnleiting.top

TS:   await fetch(url)
来源：http://zht.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://inh.cheryme.top

Go:   resp, err := http.Get(url)
来源：http://zeg.fanxiaobao.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://pht.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://atu.redwolf501.top

[L02] 发送 POST JSON
来源：http://tpe.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://kcd.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fka.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cgx.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dwn.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yde.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gpo.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sbq.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xlq.tianlin.xyz

[L03] 设置自定义请求头
来源：http://fqx.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hst.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://adf.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://flz.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bdx.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://udu.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://joi.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gop.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://col.zhengqikj.top

[L04] 设置超时
来源：http://mhk.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://hbr.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ysw.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oyc.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vgs.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dwx.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://apn.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fmr.fzhhl.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kzy.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://yte.ehwqpu.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://buc.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zsz.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nai.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://muk.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qoo.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yie.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jmf.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://heg.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://ibg.jinqigufen.top

Py:   resp.json()
来源：http://vpr.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://oxw.meibo888.top

JS:   await resp.json()
来源：http://uvv.ehwqpu.com

TS:   await resp.json()
来源：http://aal.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cmw.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ove.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://szv.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rkn.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://qpb.dianchejie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ahj.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yvs.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://olg.meibo888.top

TS:   resp.ok;  resp.status
来源：http://clf.cheryme.top

Java: resp.statusCode()
来源：http://rmh.chenzaomai.com

Go:   resp.StatusCode
来源：http://tzx.cucudq.cn

Ruby: resp.code.to_i
来源：http://vmr.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://ail.yuxming.cn

[L08] 并发请求多个地址
来源：http://tty.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fpm.guowangkeji.top

PHP:  curl_multi_init() 系列
来源：http://xum.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gel.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mem.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dod.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tmj.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mhf.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ubn.52xcode.cn

================================================================================
来源：http://qhy.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://qgv.sweek.top

================================================================================
来源：http://nng.sweek.top

[M01] 读取命令行参数
来源：http://feu.hnqzz.top

Py:   sys.argv[1:]
来源：http://qhb.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://gfe.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://kxr.wangdashe.top

TS:   process.argv.slice(2)
来源：http://wrc.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://yob.gotoacloud.top

Go:   os.Args[1:]
来源：http://yel.hesvh.cn

Ruby: ARGV
来源：http://wus.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://psq.sufxvd.cn

[M02] 读取环境变量
来源：http://dtk.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://bum.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kta.vqdsnc.cn

JS:   process.env.HOME
来源：http://vem.nanxinkj.top

TS:   process.env.HOME
来源：http://tju.hysaishi.cn

Java: System.getenv("HOME")
来源：http://vhq.ydzc1.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rvy.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://nba.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jnl.snrcjt.cn

[M03] 执行外部命令
来源：http://vba.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ned.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qmp.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://req.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://caj.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xiq.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ofh.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://fhw.yj20258888.top

C#:   Process.Start("ls", "-l");
来源：http://qtu.ivvv.top

[M04] 获取当前工作目录
来源：http://dhw.sweek.top

Py:   os.getcwd()
来源：http://ipx.jqgfzy.top

PHP:  getcwd();
来源：http://usl.aizwys.cn

JS:   process.cwd()
来源：http://yvc.sysykeji.top

TS:   process.cwd()
来源：http://jhm.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://gsy.hnqzz.top

Go:   os.Getwd()
来源：http://qks.meibo888.top

Ruby: Dir.pwd
来源：http://kxc.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://esb.zhengqikj.top

[M05] 设置退出码
来源：http://rzt.yvedp.cn

Py:   sys.exit(1)
来源：http://twg.hfpthk.cn

PHP:  exit(1);
来源：http://esp.havefunace.top

JS:   process.exit(1)
来源：http://scn.vqdsnc.cn

TS:   process.exit(1)
来源：http://qin.jinqigufen.top

Java: System.exit(1)
来源：http://fnh.zhengqikj.top

Go:   os.Exit(1)
来源：http://mmd.shanyushiyangkeji.top

Ruby: exit 1
来源：http://iry.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://alm.yfazqb.com

[M06] 向标准错误输出
来源：http://bgo.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://fre.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://szk.nwbrower.top

JS:   console.error("err")
来源：http://wwf.sufxvd.cn

TS:   console.error("err")
来源：http://hqs.jianghu66.top

Java: System.err.println("err")
来源：http://jio.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mxd.wangshuangyany.cn

Ruby: warn "err"
来源：http://efe.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://skk.daxiang520.top

[M07] 判断是否为主入口
来源：http://bys.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://luz.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://btd.hesvh.cn

JS:   require.main === module
来源：http://soj.snrcjt.cn

TS:   require.main === module
来源：http://uow.iojbl.cn

Java: public static void main(String[] args)
来源：http://kvg.hesvh.cn

Go:   func main()
来源：http://vxg.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mal.meibo888.top

C#:   static void Main(string[] args)
来源：http://hyy.daria6918.cn

[M08] 获取系统与运行时信息
来源：http://xxy.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://pgc.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://cmt.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://xzc.yueranfly.top

TS:   process.platform;  process.version
来源：http://aew.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ctd.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://leq.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mxb.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://phi.hesvh.cn

================================================================================
来源：http://hac.andypj.xyz

N. 数据结构与算法
来源：http://rwd.sweek.top

================================================================================
来源：http://cky.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://osp.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://apx.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kks.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dxf.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://unt.zdbjq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qvv.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://nio.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iqp.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://eno.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://dyp.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://eho.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dse.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uqf.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ppj.chenzaomai.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ifn.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://clv.zhongyouzk.top

Ruby: arr.sort
来源：http://rtu.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vvp.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://xee.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mqp.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://kxg.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://shd.fzhhl.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yke.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://stz.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jpd.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://thc.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://ota.fktsv.cn

[N04] 斐波那契数列
来源：http://fbt.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fdu.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pfd.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gsh.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vwd.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cda.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dqr.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lbr.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://arc.jqgufenzy.top

[N05] 最大公约数
来源：http://coj.cheryme.top

Py:   math.gcd(a, b)
来源：http://ngm.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xzn.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jrs.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jic.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hyo.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eqy.shuidangran.top

Ruby: a.gcd(b)
来源：http://vky.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nin.yfazqb.com

[N06] 判断回文字符串
来源：http://fbv.hfpthk.cn

Py:   s == s[::-1]
来源：http://gmt.hnqzz.top

PHP:  $s === strrev($s);
来源：http://piq.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://saf.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://fnf.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://idr.yvedp.cn

Go:   // 双指针从两端比较
来源：http://rdh.jianghu66.top

Ruby: s == s.reverse
来源：http://dbb.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sfz.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://rsw.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uhj.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ces.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yea.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://geg.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://jst.cheryme.top

Go:   // 手写 map[int]int
来源：http://dds.52xcode.cn

Ruby: // 手写 Hash
来源：http://yzg.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://cmw.hfpthk.cn

[N08] 生成全排列
来源：http://zms.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://ajw.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://hne.sweek.top

JS:   // 手写回溯递归
来源：http://vxn.dashuyun.cn

TS:   // 手写回溯递归
来源：http://jcf.uphjek.com

Java: // 手写回溯递归
来源：http://zqv.daxiang520.top

Go:   // 手写回溯递归
来源：http://qwe.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://cfh.chenzaomai.com

C#:   // 手写回溯递归
来源：http://svp.shuidangran.top

[N09] 栈与队列
来源：http://wmo.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xqm.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xkj.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mbx.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cpf.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tuf.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gtn.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bss.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wsy.cdnleiting.top

[N10] 链表节点定义
来源：http://kyn.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gue.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://toa.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wzr.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sny.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://pup.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://esg.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ayc.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wrs.316326.xyz

[N11] 二叉树中序遍历
来源：http://fxf.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kit.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://gfe.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bht.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nkf.vehdjk.com

Java: // 手写递归
来源：http://kxa.c1oappe.top

Go:   // 手写递归
来源：http://szz.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bqi.daxiang520.top

C#:   // 手写递归
来源：http://yfz.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nrj.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qju.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oji.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qrx.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xuj.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pie.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qal.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jbi.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://off.guannengcc.top

================================================================================
来源：http://tfz.tian-w.cn

O. 并发与异步
来源：http://szl.aizwys.cn

================================================================================
来源：http://kod.cucudq.cn

[O01] 启动一个线程
来源：http://pyv.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rqo.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://luu.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cmz.dianchejie.cn

TS:   // 同 JS
来源：http://mhr.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://rzr.hysaishi.cn

Go:   go f()
来源：http://xox.andypj.xyz

Ruby: Thread.new { f }
来源：http://xcc.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://xyp.dashuyun.cn

[O02] 使用线程池
来源：http://vbq.ybcxt.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fjo.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://npw.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://upn.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://qup.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xpy.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://npi.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xuu.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zpo.wangdashe.top

[O03] 加锁保护共享数据
来源：http://rgr.guowangkeji.top

Py:   with lock: shared += 1
来源：http://vxk.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://cvr.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jcl.ehwqpu.com

TS:   // 同 JS
来源：http://zqb.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://wat.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://efc.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yft.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://bel.yueranfly.top

[O04] 定义异步函数并等待
来源：http://bgx.meibo888.top

Py:   async def f():⏎    await g()
来源：http://uuo.zhixingplan.top


<!-- 参考信息 -->