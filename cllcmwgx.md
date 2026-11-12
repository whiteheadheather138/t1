代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://axe.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kwj.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ksn.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wen.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pvj.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ehy.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://gqg.zhiwuduotai.top

Py:   pickle.dumps(obj)
来源：http://cgn.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yud.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://pwb.cashguo.top

TS:   v8.serialize(obj)        // Node
来源：http://wzs.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kwq.yj20258888.top

Go:   encoding/gob
来源：http://esr.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://hch.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bxh.birdmap.top

================================================================================
来源：http://pam.zhiwuduotai.top

L. 网络请求
来源：http://zns.zycfv.cn

================================================================================
来源：http://euj.hywenlv.cn

[L01] 发送 GET 请求
来源：http://ecq.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fbu.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vgz.wangshuangyany.cn

JS:   await fetch(url)
来源：http://vcx.yfazqb.com

TS:   await fetch(url)
来源：http://fmf.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hjb.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://tks.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hha.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://swk.wangdashe.top

[L02] 发送 POST JSON
来源：http://uke.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cjf.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dvl.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jvt.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mph.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nez.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dwg.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://juy.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bnr.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://jff.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jrn.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yqa.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ate.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wvl.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aab.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kpi.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pcm.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gpj.shzxlz.cn

[L04] 设置超时
来源：http://mgv.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://ykg.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ncl.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ois.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://brp.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bjv.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://guo.shzxlz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://skk.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nme.xuanzx.com

[L05] 上传文件（multipart）
来源：http://uvk.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sch.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wvt.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://epc.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xxm.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kqy.ybcxt.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xui.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dup.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vbf.jianghu66.top

[L06] 解析响应为 JSON
来源：http://lro.yvedp.cn

Py:   resp.json()
来源：http://ttn.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://wwb.fanxiaobao.xyz

JS:   await resp.json()
来源：http://wdq.pycfn.com

TS:   await resp.json()
来源：http://tct.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gkh.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eef.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://wtq.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fpb.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://bii.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ktf.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zdy.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://wcd.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://yql.zhiwuduotai.top

Java: resp.statusCode()
来源：http://mes.hnxiangtu.top

Go:   resp.StatusCode
来源：http://itk.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://nid.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://dkd.316326.xyz

[L08] 并发请求多个地址
来源：http://nbu.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wyv.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://voo.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jfp.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gkz.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dgj.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://myi.zhongyouzk.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aew.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ptq.hammf.cn

================================================================================
来源：http://hxh.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://svu.hammf.cn

================================================================================
来源：http://saf.yanxiufei.cn

[M01] 读取命令行参数
来源：http://wwm.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://vgn.yueranfly.top

PHP:  $argv;  $argc;
来源：http://qho.birdmap.top

JS:   process.argv.slice(2)
来源：http://jfu.sxryk.cn

TS:   process.argv.slice(2)
来源：http://xtq.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://azh.cashguo.top

Go:   os.Args[1:]
来源：http://xtv.shanyushiyangtech.top

Ruby: ARGV
来源：http://vav.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://vpo.bjfxy.top

[M02] 读取环境变量
来源：http://rvs.uphjek.com

Py:   os.environ.get("HOME")
来源：http://eut.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://moe.gaohongyu789.top

JS:   process.env.HOME
来源：http://bre.hcnkem.com

TS:   process.env.HOME
来源：http://lwc.nanxuanxn.top

Java: System.getenv("HOME")
来源：http://yfe.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lfl.andypj.xyz

Ruby: ENV["HOME"]
来源：http://zln.yj20258.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lrg.nanxuanxn.top

[M03] 执行外部命令
来源：http://cll.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xll.9152youxi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rzf.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xdg.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wkt.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ssm.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lhi.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://hpx.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://tak.sweek.top

[M04] 获取当前工作目录
来源：http://dfe.zhiwuduotai.top

Py:   os.getcwd()
来源：http://hgq.hnxiangtu.top

PHP:  getcwd();
来源：http://rwm.haohaochexian.top

JS:   process.cwd()
来源：http://pwd.ehwqpu.com

TS:   process.cwd()
来源：http://urk.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://krb.ywan-chungtsiang.top

Go:   os.Getwd()
来源：http://eam.cqqwz.cn

Ruby: Dir.pwd
来源：http://jvp.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://mmi.nanxuanxn.top

[M05] 设置退出码
来源：http://utc.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://wup.nwbrower.top

PHP:  exit(1);
来源：http://ker.yuanzhike.top

JS:   process.exit(1)
来源：http://sbt.shangyingyoupin.top

TS:   process.exit(1)
来源：http://hmj.ybcxt.top

Java: System.exit(1)
来源：http://kll.guowangkeji.top

Go:   os.Exit(1)
来源：http://vwo.nanxuanxn.top

Ruby: exit 1
来源：http://nqz.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xwd.cdnleiting.top

[M06] 向标准错误输出
来源：http://lwv.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://tre.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zgo.daxiang520.top

JS:   console.error("err")
来源：http://kpy.chenzaomai.com

TS:   console.error("err")
来源：http://eiw.cdnleiting.top

Java: System.err.println("err")
来源：http://lou.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fuf.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://qrz.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://mvn.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://vzq.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://pvs.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ukh.tanke756.top

JS:   require.main === module
来源：http://vnf.zycfv.cn

TS:   require.main === module
来源：http://mfi.cheryme.top

Java: public static void main(String[] args)
来源：http://fxj.ybcxt.top

Go:   func main()
来源：http://wfw.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qhw.yvedp.cn

C#:   static void Main(string[] args)
来源：http://ehy.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://ahm.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://hvk.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://jot.ybcxt.top

JS:   process.platform;  process.version
来源：http://wkq.sweek.top

TS:   process.platform;  process.version
来源：http://uun.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nsb.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hby.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ykt.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://poe.yanxiufei.cn

================================================================================
来源：http://nmt.svipenyu.cn

N. 数据结构与算法
来源：http://yja.hongshengwenyu.top

================================================================================
来源：http://rkh.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://sug.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://fon.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kbk.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpc.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://alu.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://xxd.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://xff.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iuu.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://bdw.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://bct.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://plv.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nsp.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dae.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fnn.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wfv.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://nrl.yj20258.top

Ruby: arr.sort
来源：http://jer.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tfb.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://tdt.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ynh.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://dtt.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zti.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yya.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pjr.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tsd.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lsr.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://tsj.c1oappe.top

[N04] 斐波那契数列
来源：http://rjh.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oqw.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ubo.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wwa.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qec.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dim.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wyj.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aws.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qrb.gotoacloud.top

[N05] 最大公约数
来源：http://mtf.hesvh.cn

Py:   math.gcd(a, b)
来源：http://iim.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ssm.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blg.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gbx.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pyr.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qip.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://eay.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wed.316326.xyz

[N06] 判断回文字符串
来源：http://zqp.guowangkeji.top

Py:   s == s[::-1]
来源：http://wap.smart0.xyz

PHP:  $s === strrev($s);
来源：http://yug.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://yve.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://ayz.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wpb.wangdashe.top

Go:   // 双指针从两端比较
来源：http://tog.shuidangran.top

Ruby: s == s.reverse
来源：http://kkh.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gfz.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://oed.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lri.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://evf.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://umt.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://ddw.yfazqb.com

Java: // 手写 HashMap
来源：http://iii.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://vrq.pycfn.com

Ruby: // 手写 Hash
来源：http://rgc.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://vkg.cqqwz.cn

[N08] 生成全排列
来源：http://ttj.yongpay.top

Py:   itertools.permutations(arr)
来源：http://sed.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://zfb.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://xud.gogol.net.cn

TS:   // 手写回溯递归
来源：http://jor.sweek.top

Java: // 手写回溯递归
来源：http://bbz.hysaishi.cn

Go:   // 手写回溯递归
来源：http://dgi.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://omh.ctjpmb.com

C#:   // 手写回溯递归
来源：http://bqr.gotoacloud.top

[N09] 栈与队列
来源：http://grj.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mik.nanxuanxn.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://egj.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vhw.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gpa.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rxe.shuidangran.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cni.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uor.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ziw.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://cwv.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kxt.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://drj.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ppi.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ohs.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://xnz.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://rty.daria6918.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ebd.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rbk.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://xlz.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tbd.sufxvd.cn

PHP:  // 手写递归函数
来源：http://ugy.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ght.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fjb.chenzaomai.com

Java: // 手写递归
来源：http://kyz.9152youxi.cn

Go:   // 手写递归
来源：http://xkt.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xgq.cdnleiting.top

C#:   // 手写递归
来源：http://aed.kuanghao11.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xbu.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fmp.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nzb.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tml.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bye.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://otk.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sty.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ziw.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xcn.shanyushiyangkeji.top

================================================================================
来源：http://sqz.jlsjyb.cn

O. 并发与异步
来源：http://sff.chenlongwang.top

================================================================================
来源：http://wey.yfazqb.com

[O01] 启动一个线程
来源：http://yjl.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yzr.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gxk.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mhq.birdmap.top

TS:   // 同 JS
来源：http://bps.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://api.jqgfzy.top

Go:   go f()
来源：http://phb.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://gjk.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://ioo.snrcjt.cn

[O02] 使用线程池
来源：http://zfx.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kfu.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nre.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://gka.tianlin.xyz

TS:   // worker_threads 线程池
来源：http://iwa.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://npf.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zkl.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sph.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jsy.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://aku.yj20258.top

Py:   with lock: shared += 1
来源：http://swu.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://usy.haohaochexian.top


<!-- 参考信息 -->