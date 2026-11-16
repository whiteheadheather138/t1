代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gdt.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kll.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qxk.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kzn.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xin.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zkc.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://hkp.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://rkn.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zzp.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://zxk.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://cri.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pjq.zdqjudy.top

Go:   encoding/gob
来源：http://alf.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://ker.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rma.feifeiyinyue.top

================================================================================
来源：http://hxj.jinqigfzy.top

L. 网络请求
来源：http://hus.yongpay.top

================================================================================
来源：http://csj.fktsv.cn

[L01] 发送 GET 请求
来源：http://nmf.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zww.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rha.xuetiantiany.cn

JS:   await fetch(url)
来源：http://zpe.fktsv.cn

TS:   await fetch(url)
来源：http://wtm.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lfy.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://bsa.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wih.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://swj.sweek.top

[L02] 发送 POST JSON
来源：http://reh.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://oxq.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://erm.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qbn.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://isu.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vcl.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vma.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hyd.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sbo.cucudq.cn

[L03] 设置自定义请求头
来源：http://frf.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tra.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jdi.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://urz.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gbt.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kuw.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gdf.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vkn.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lob.yongpay.top

[L04] 设置超时
来源：http://rnw.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://yzd.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rrh.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://asm.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nif.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iqo.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wbb.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yor.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tye.hywenlv.cn

[L05] 上传文件（multipart）
来源：http://qng.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ymm.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fle.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ouf.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xds.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yst.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://krl.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xqi.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jhc.bbcook.cn

[L06] 解析响应为 JSON
来源：http://agy.c1oappe.top

Py:   resp.json()
来源：http://ivz.tanke756.top

PHP:  json_decode($body, true);
来源：http://nvn.bbcook.cn

JS:   await resp.json()
来源：http://yxt.redwolf501.top

TS:   await resp.json()
来源：http://xqe.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fbw.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oar.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://mlk.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://exx.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://zgy.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ejg.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nrj.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://pkv.pycfn.com

TS:   resp.ok;  resp.status
来源：http://mih.redwolf501.top

Java: resp.statusCode()
来源：http://wql.yj20258888.top

Go:   resp.StatusCode
来源：http://rln.yfazqb.com

Ruby: resp.code.to_i
来源：http://bns.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://ixn.sufxvd.cn

[L08] 并发请求多个地址
来源：http://oue.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vce.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://oga.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iqg.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sdm.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xhq.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qhn.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fuh.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fzv.dianchejie.cn

================================================================================
来源：http://abn.xuetiantiany.cn

M. 命令行 / 进程 / 环境
来源：http://tns.0kj1m.cn

================================================================================
来源：http://rgp.jqgfzy.top

[M01] 读取命令行参数
来源：http://vxa.daxiang520.top

Py:   sys.argv[1:]
来源：http://uia.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://mxu.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://qfn.cucudq.cn

TS:   process.argv.slice(2)
来源：http://ynk.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://ukt.gotoacloud.top

Go:   os.Args[1:]
来源：http://dlh.yj20258888.top

Ruby: ARGV
来源：http://bhw.yuanzhike.top

C#:   args 数组（Main 方法参数）
来源：http://nff.ybcxt.top

[M02] 读取环境变量
来源：http://mnj.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://aug.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lqo.jiagoushi.top

JS:   process.env.HOME
来源：http://gpm.aizwys.cn

TS:   process.env.HOME
来源：http://ukx.ivvv.top

Java: System.getenv("HOME")
来源：http://reb.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zpl.pycfn.com

Ruby: ENV["HOME"]
来源：http://nii.yuxming.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://stf.ivvv.top

[M03] 执行外部命令
来源：http://cph.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ytj.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ygw.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://icf.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ogl.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xgy.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://txv.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://qqg.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://xcy.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://jrz.aibaodan.cn

Py:   os.getcwd()
来源：http://zwq.wangdashe.top

PHP:  getcwd();
来源：http://kpa.zhiwuduotai.top

JS:   process.cwd()
来源：http://xgc.yuxming.cn

TS:   process.cwd()
来源：http://jgj.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://uhy.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://qcz.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://ktl.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://cgg.yvedp.cn

[M05] 设置退出码
来源：http://lzi.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://lsy.jinghuilouyu.cn

PHP:  exit(1);
来源：http://mph.birdmap.top

JS:   process.exit(1)
来源：http://ihz.jianghu66.top

TS:   process.exit(1)
来源：http://sqb.xinyue.icu

Java: System.exit(1)
来源：http://ana.zdqjudy.top

Go:   os.Exit(1)
来源：http://koa.shanyushiyangkeji.top

Ruby: exit 1
来源：http://zel.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xfz.316326.xyz

[M06] 向标准错误输出
来源：http://san.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://xlf.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sii.jlsjyb.cn

JS:   console.error("err")
来源：http://zmu.jqgufenzy.top

TS:   console.error("err")
来源：http://mdg.quarkkingdee.top

Java: System.err.println("err")
来源：http://kdj.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pwy.shuidangran.top

Ruby: warn "err"
来源：http://rwt.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://auk.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://pop.yvedp.cn

Py:   if __name__ == "__main__":
来源：http://cve.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://plu.jinghuilouyu.cn

JS:   require.main === module
来源：http://yje.guannengcc.top

TS:   require.main === module
来源：http://bva.yj20258888.top

Java: public static void main(String[] args)
来源：http://jtq.cqqwz.cn

Go:   func main()
来源：http://fce.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://llt.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://wdi.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://zqo.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://ubd.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://qix.bjfxy.top

JS:   process.platform;  process.version
来源：http://bxp.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://sms.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vat.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bgt.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zwr.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://otw.daria6918.cn

================================================================================
来源：http://ebk.hfpthk.cn

N. 数据结构与算法
来源：http://cgp.jinyuanbaomall.cn

================================================================================
来源：http://jsn.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://fqw.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://oue.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mzv.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bav.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kcx.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://rwp.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://uko.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nfa.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ydg.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://alg.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://lfq.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://paq.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mpx.sjlbkw.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cre.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ihj.fehbvm.com

Go:   slices.Sort(arr)
来源：http://euo.jqgfzy.top

Ruby: arr.sort
来源：http://mry.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ncd.cashguo.top

[N03] 快速排序（分治示例）
来源：http://bll.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kbs.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://knr.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://flx.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kgy.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yeg.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mik.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rtu.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://jga.daxiang520.top

[N04] 斐波那契数列
来源：http://uyb.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fbf.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fgy.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xiu.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fyc.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ouf.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gdn.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://udi.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pvw.sxryk.cn

[N05] 最大公约数
来源：http://eto.sysykeji.top

Py:   math.gcd(a, b)
来源：http://irs.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qes.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://san.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wob.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ykj.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://orh.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://iqg.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ant.zhengqikj.top

[N06] 判断回文字符串
来源：http://sls.wangdashe.top

Py:   s == s[::-1]
来源：http://unw.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://ejq.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://rgs.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://ijt.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wao.cashguo.top

Go:   // 双指针从两端比较
来源：http://avw.feifeiyinyue.top

Ruby: s == s.reverse
来源：http://nza.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cif.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://xsz.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ysf.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bsq.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dmk.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://cfy.tian-w.cn

Java: // 手写 HashMap
来源：http://scj.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://cqk.daxiang520.top

Ruby: // 手写 Hash
来源：http://hkj.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fgv.52xcode.cn

[N08] 生成全排列
来源：http://nav.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://hrz.sufxvd.cn

PHP:  // 手写递归交换
来源：http://jff.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://wdk.aibaodan.cn

TS:   // 手写回溯递归
来源：http://jef.jiagoushi.top

Java: // 手写回溯递归
来源：http://uqx.gogol.net.cn

Go:   // 手写回溯递归
来源：http://yqz.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://vbi.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://ieb.xziqi.cn

[N09] 栈与队列
来源：http://obh.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jyg.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jni.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wuf.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sse.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hec.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lmr.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iwz.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wyn.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://dre.hfpthk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xel.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cvg.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dio.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://suk.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://jwz.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tiq.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rro.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://etm.hesvh.cn

[N11] 二叉树中序遍历
来源：http://wod.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xmi.hesvh.cn

PHP:  // 手写递归函数
来源：http://nsc.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://txw.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wle.zhiwuduotai.top

Java: // 手写递归
来源：http://qfj.cashguo.top

Go:   // 手写递归
来源：http://jfm.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qoh.sxryk.cn

C#:   // 手写递归
来源：http://pmr.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eyo.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cwd.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pfp.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wbe.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fki.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://imp.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ave.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eco.zhongyouzk.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ouu.c1oappe.top

================================================================================
来源：http://epr.redwolf501.top

O. 并发与异步
来源：http://tox.daxiang520.top

================================================================================
来源：http://qai.hywenlv.cn

[O01] 启动一个线程
来源：http://jzx.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sbx.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ngr.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qus.sxryk.cn

TS:   // 同 JS
来源：http://rfx.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://ftp.jinghuilouyu.cn

Go:   go f()
来源：http://iik.gzhubu.top

Ruby: Thread.new { f }
来源：http://inr.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://fxm.epnwcf.com

[O02] 使用线程池
来源：http://ntb.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zsl.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://whm.hesvh.cn

JS:   // worker_threads 线程池
来源：http://ata.shangyingyoupin.top

TS:   // worker_threads 线程池
来源：http://wiw.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://kcx.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kyw.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tmu.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kza.c1oappe.top

[O03] 加锁保护共享数据
来源：http://dxu.nanxinkj.top

Py:   with lock: shared += 1
来源：http://cjt.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://zwb.zycfv.cn


<!-- 参考信息 -->