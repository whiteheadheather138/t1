代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rar.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jzh.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://bld.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://mda.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rlh.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://hwb.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://qeg.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://isk.hongshengwenyu.top

Go:   encoding/gob
来源：http://vma.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://oot.zhiwuduotai.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dbg.hnqzz.top

================================================================================
来源：http://ove.shzxlz.cn

L. 网络请求
来源：http://css.yanxiufei.cn

================================================================================
来源：http://ajp.uphjek.com

[L01] 发送 GET 请求
来源：http://vvz.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vxq.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jkq.shzxlz.cn

JS:   await fetch(url)
来源：http://krc.nanxinkj.top

TS:   await fetch(url)
来源：http://wqy.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qxe.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://vmn.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dsp.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vre.sxryk.cn

[L02] 发送 POST JSON
来源：http://fvg.fzhhl.top

Py:   requests.post(url, json={"a": 1})
来源：http://fjz.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jbi.9152youxi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://awa.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kqx.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aei.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nfd.sysykeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xzg.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cdm.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://vdc.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pmt.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ksz.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ggt.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hxq.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ioq.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://psd.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ida.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ozz.xinyue.icu

[L04] 设置超时
来源：http://fde.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://tlx.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qrc.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yzl.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hgy.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://veq.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bak.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://olx.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tir.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://msm.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://toz.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kim.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lbw.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jpw.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dst.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gad.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eif.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gmk.ydzc1.top

[L06] 解析响应为 JSON
来源：http://nmj.hcnkem.com

Py:   resp.json()
来源：http://aop.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://sku.tianlin.xyz

JS:   await resp.json()
来源：http://bsn.ydzc1.top

TS:   await resp.json()
来源：http://vgn.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://okv.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xct.hammf.cn

Ruby: JSON.parse(resp.body)
来源：http://bsm.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fdm.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://csv.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jwj.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ccd.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://xpq.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://egm.xziqi.cn

Java: resp.statusCode()
来源：http://bdl.quarkkingdee.top

Go:   resp.StatusCode
来源：http://khz.9152youxi.cn

Ruby: resp.code.to_i
来源：http://glt.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://mhf.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://rvx.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xnp.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://hmh.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oea.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qib.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iwy.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://coi.cdnleiting.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qrh.yanxiufei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gkv.daxiang520.top

================================================================================
来源：http://kan.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://rqv.chenjidiqi.icu

================================================================================
来源：http://ixv.zycfv.cn

[M01] 读取命令行参数
来源：http://eqy.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://yhb.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://doz.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://rgx.ivvv.top

TS:   process.argv.slice(2)
来源：http://okm.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://mqz.yuxming.cn

Go:   os.Args[1:]
来源：http://qkf.hywenlv.cn

Ruby: ARGV
来源：http://tgn.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://opf.fengsongda.top

[M02] 读取环境变量
来源：http://znu.yongpay.top

Py:   os.environ.get("HOME")
来源：http://jjk.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://str.nwbrower.top

JS:   process.env.HOME
来源：http://rco.jlsjyb.cn

TS:   process.env.HOME
来源：http://xty.yuanzhike.top

Java: System.getenv("HOME")
来源：http://zck.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zsd.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://nqz.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://izj.feifeiyinyue.top

[M03] 执行外部命令
来源：http://urf.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cjl.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dyl.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qfc.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kzh.gotoacloud.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://czs.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ach.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://mve.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://agu.daxiang520.top

[M04] 获取当前工作目录
来源：http://pnh.hammf.cn

Py:   os.getcwd()
来源：http://ejm.hongshengwenyu.top

PHP:  getcwd();
来源：http://owb.zhongyouzk.top

JS:   process.cwd()
来源：http://xeg.zycfv.cn

TS:   process.cwd()
来源：http://fzi.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://eux.jlsjyb.cn

Go:   os.Getwd()
来源：http://ihj.zhengqikj.top

Ruby: Dir.pwd
来源：http://rtc.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://umb.quarkkingdee.top

[M05] 设置退出码
来源：http://hwr.jiagoushi.top

Py:   sys.exit(1)
来源：http://kvz.kuanghao11.cn

PHP:  exit(1);
来源：http://jhl.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://wur.zdqjudy.top

TS:   process.exit(1)
来源：http://jie.fktsv.cn

Java: System.exit(1)
来源：http://ddr.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://crc.zhongyouzk.top

Ruby: exit 1
来源：http://fyc.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nii.shuidangran.top

[M06] 向标准错误输出
来源：http://pxr.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://tus.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://laj.shuidangran.top

JS:   console.error("err")
来源：http://tkq.zhoulong.xyz

TS:   console.error("err")
来源：http://nsu.yj20258888.top

Java: System.err.println("err")
来源：http://dpz.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dlo.mhx1999.top

Ruby: warn "err"
来源：http://uak.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://koj.jianghu66.top

[M07] 判断是否为主入口
来源：http://fmm.meibo888.top

Py:   if __name__ == "__main__":
来源：http://xuz.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tmb.hfpthk.cn

JS:   require.main === module
来源：http://rnt.nanxinkj.top

TS:   require.main === module
来源：http://dpa.yuxming.cn

Java: public static void main(String[] args)
来源：http://qed.ehwqpu.com

Go:   func main()
来源：http://gir.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dbm.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://ncy.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://rop.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://gqz.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://vlc.hesvh.cn

JS:   process.platform;  process.version
来源：http://jbq.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://vzc.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ept.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hnw.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gzf.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vpp.bbcook.cn

================================================================================
来源：http://tby.ydjk.org.cn

N. 数据结构与算法
来源：http://qhz.sxryk.cn

================================================================================
来源：http://eua.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://hah.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://bfa.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wma.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rok.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mys.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pxc.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://xmw.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nju.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ibj.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://bxb.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://jyg.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pih.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ktk.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cuq.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://abi.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://kbp.gaohongyu789.top

Ruby: arr.sort
来源：http://sgs.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xza.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://tbu.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qzj.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://fpw.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mgl.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tdm.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cxb.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kps.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iae.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://sbd.gaohongyu789.top

[N04] 斐波那契数列
来源：http://uhs.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nao.jqgfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vsi.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kvo.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vcc.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://plk.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ush.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nct.chenzaomai.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yqt.hnxiangtu.top

[N05] 最大公约数
来源：http://tnb.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://ctv.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://trw.ybcxt.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://evg.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sif.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sdp.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://axt.yonumen.top

Ruby: a.gcd(b)
来源：http://hzy.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cys.0kj1m.cn

[N06] 判断回文字符串
来源：http://llh.yuanzhike.top

Py:   s == s[::-1]
来源：http://svx.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://dub.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://ieu.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://snb.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gjl.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://rzz.hfpthk.cn

Ruby: s == s.reverse
来源：http://ycd.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xxv.yvedp.cn

[N07] 两数之和（返回下标）
来源：http://ptc.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sqk.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://obn.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pqj.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://iam.fktsv.cn

Java: // 手写 HashMap
来源：http://jqg.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://wyt.ybcxt.top

Ruby: // 手写 Hash
来源：http://yrl.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xtk.cashguo.top

[N08] 生成全排列
来源：http://gxq.cashguo.top

Py:   itertools.permutations(arr)
来源：http://pzy.zycfv.cn

PHP:  // 手写递归交换
来源：http://bkt.zhixingplan.top

JS:   // 手写回溯递归
来源：http://vqc.svipenyu.cn

TS:   // 手写回溯递归
来源：http://fmh.jqgfzy.top

Java: // 手写回溯递归
来源：http://pyf.cashguo.top

Go:   // 手写回溯递归
来源：http://ezl.yonumen.top

Ruby: arr.permutation.to_a
来源：http://rox.c1oappe.top

C#:   // 手写回溯递归
来源：http://uwp.ehwqpu.com

[N09] 栈与队列
来源：http://nuc.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zst.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iti.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iih.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gqx.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zgq.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pvf.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://brc.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://egz.ydzc1.top

[N10] 链表节点定义
来源：http://yfk.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kgf.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xbi.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yke.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aws.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://xdv.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://mts.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ths.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xrh.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://pqa.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lsp.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://acp.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xhz.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://otg.ydjk.org.cn

Java: // 手写递归
来源：http://aad.tianlin.xyz

Go:   // 手写递归
来源：http://fiy.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wgm.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://tae.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aou.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mzo.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sgl.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://crh.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nld.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zpu.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zjg.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xag.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hot.52xcode.cn

================================================================================
来源：http://zde.andypj.xyz

O. 并发与异步
来源：http://jxt.sjlbkw.cn

================================================================================
来源：http://ehg.yj202588.top

[O01] 启动一个线程
来源：http://wgo.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nsw.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ynd.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eec.yj202588.top

TS:   // 同 JS
来源：http://jdj.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://jbs.cdnleiting.top

Go:   go f()
来源：http://cat.yueranfly.top

Ruby: Thread.new { f }
来源：http://vxa.sweek.top

C#:   Task.Run(() => F());
来源：http://ahu.nanxuanxn.top

[O02] 使用线程池
来源：http://wec.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pjo.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cqf.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://qoe.iojbl.cn

TS:   // worker_threads 线程池
来源：http://xsf.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://lvj.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nxg.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qcd.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wbb.tanke756.top

[O03] 加锁保护共享数据
来源：http://fbm.ctjpmb.com

Py:   with lock: shared += 1
来源：http://ste.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://rni.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://chl.yj202588.top

TS:   // 同 JS
来源：http://sry.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://vko.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wab.sjlbkw.cn


<!-- 参考信息 -->