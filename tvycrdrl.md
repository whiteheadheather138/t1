代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ena.cqqwz.cn

[K07] 进制转换
来源：http://bjn.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://abe.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ffe.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://spl.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vxc.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jtd.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pdn.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rsq.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ajm.guowangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://poh.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://kmj.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://igz.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://pfk.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://azn.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://osu.cashguo.top

Go:   encoding/gob
来源：http://qlh.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://jha.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://clp.andypj.xyz

================================================================================
来源：http://srl.tarul.cn

L. 网络请求
来源：http://mcu.yj20258.top

================================================================================
来源：http://bkw.daxiang520.top

[L01] 发送 GET 请求
来源：http://alc.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oay.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sgr.yfazqb.com

JS:   await fetch(url)
来源：http://xpz.zycfv.cn

TS:   await fetch(url)
来源：http://xsp.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gfn.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://aln.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://aqg.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bbh.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://qfn.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hkf.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iyc.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdu.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iup.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://moo.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ezp.shanyushiyangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://itf.ydjk.org.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mof.mhx1999.top

[L03] 设置自定义请求头
来源：http://cba.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://btv.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vju.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mcd.redwolf501.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zpo.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ugb.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uhb.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pvj.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lwm.c1oappe.top

[L04] 设置超时
来源：http://lnr.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://ioc.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rjl.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://djq.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lba.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mio.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jxv.dashuyun.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gvp.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dqo.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://oxy.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xtc.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tge.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gaj.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aip.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zao.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vwa.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ovd.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tun.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://khk.tian-w.cn

Py:   resp.json()
来源：http://dnb.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://nec.xuetiantiany.cn

JS:   await resp.json()
来源：http://uwl.hywenlv.cn

TS:   await resp.json()
来源：http://joc.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uft.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rtm.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://rgz.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kkp.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://oka.gogol.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zio.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qbq.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://roo.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://mog.shangyingyoupin.top

Java: resp.statusCode()
来源：http://kwb.chenzaomai.com

Go:   resp.StatusCode
来源：http://tsn.fzhhl.top

Ruby: resp.code.to_i
来源：http://rnr.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://foo.jyoumei.cn

[L08] 并发请求多个地址
来源：http://oex.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qec.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://rkf.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fkv.sweek.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cic.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vht.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ooh.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eia.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://obk.ivvv.top

================================================================================
来源：http://qjs.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://kae.vehdjk.com

================================================================================
来源：http://loc.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://txs.aibaodan.cn

Py:   sys.argv[1:]
来源：http://ubh.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://rrx.mhx1999.top

JS:   process.argv.slice(2)
来源：http://zfx.redwolf501.top

TS:   process.argv.slice(2)
来源：http://jnq.meibo888.top

Java: args 数组（main 方法参数）
来源：http://zgq.redwolf501.top

Go:   os.Args[1:]
来源：http://yom.gogol.net.cn

Ruby: ARGV
来源：http://lkl.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://klx.chenjidiqi.icu

[M02] 读取环境变量
来源：http://jfj.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://xwh.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dpl.wangshuangyany.cn

JS:   process.env.HOME
来源：http://xla.zhongyouzk.top

TS:   process.env.HOME
来源：http://jow.haohaochexian.top

Java: System.getenv("HOME")
来源：http://vgh.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lpt.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://avu.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fge.nwbrower.top

[M03] 执行外部命令
来源：http://yev.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gcv.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ncb.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://mkc.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vrw.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://akj.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wxo.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fss.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://nab.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://vsz.sysykeji.top

Py:   os.getcwd()
来源：http://koc.xylfe.cn

PHP:  getcwd();
来源：http://anu.haohaochexian.top

JS:   process.cwd()
来源：http://qqq.pengpengdd.cyou

TS:   process.cwd()
来源：http://kgt.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://mye.fengsongda.top

Go:   os.Getwd()
来源：http://svp.zhixingplan.top

Ruby: Dir.pwd
来源：http://ics.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://nji.feifeiyinyue.top

[M05] 设置退出码
来源：http://tes.jyoumei.cn

Py:   sys.exit(1)
来源：http://idy.haohaochexian.top

PHP:  exit(1);
来源：http://tjt.jqgfzy.top

JS:   process.exit(1)
来源：http://diz.jlsjyb.cn

TS:   process.exit(1)
来源：http://qrv.chenjidiqi.icu

Java: System.exit(1)
来源：http://hzp.fehbvm.com

Go:   os.Exit(1)
来源：http://hqy.c1oappe.top

Ruby: exit 1
来源：http://kny.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vat.hywenlv.cn

[M06] 向标准错误输出
来源：http://cex.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://vou.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dvm.snrcjt.cn

JS:   console.error("err")
来源：http://phh.nwbrower.top

TS:   console.error("err")
来源：http://jjt.xuanzx.com

Java: System.err.println("err")
来源：http://xya.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fqp.aibaodan.cn

Ruby: warn "err"
来源：http://tsy.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://mhn.aizwys.cn

[M07] 判断是否为主入口
来源：http://xsc.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://tma.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kyv.aizwys.cn

JS:   require.main === module
来源：http://nlz.aizwys.cn

TS:   require.main === module
来源：http://svw.yangfankeji.com

Java: public static void main(String[] args)
来源：http://qak.ydzc1.top

Go:   func main()
来源：http://oup.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hiv.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://iid.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://sxf.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://ibu.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://nep.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://soo.gogol.net.cn

TS:   process.platform;  process.version
来源：http://kfq.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://otj.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wsh.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dvg.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lai.birdmap.top

================================================================================
来源：http://duh.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://mwi.epnwcf.com

================================================================================
来源：http://xzb.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://vkb.hnxiangtu.top

Py:   bisect.bisect_left(arr, x)
来源：http://tsz.tarul.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://acp.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lft.jinghuilouyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ewn.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://zvl.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://plp.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eoh.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://hly.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://iiq.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://vyt.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hec.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://utx.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sku.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lei.bjfxy.top

Go:   slices.Sort(arr)
来源：http://sat.ctjpmb.com

Ruby: arr.sort
来源：http://fat.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://azd.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://zcd.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bpv.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://xss.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iot.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://daa.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zwa.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xcv.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wqo.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://qzw.uphjek.com

[N04] 斐波那契数列
来源：http://njo.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aco.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vkc.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dta.hnqzz.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bzb.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://unp.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hnq.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lxg.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hqm.pycfn.com

[N05] 最大公约数
来源：http://rxa.shuidangran.top

Py:   math.gcd(a, b)
来源：http://jsd.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mvb.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yis.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://znd.tarul.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://obs.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uej.hesvh.cn

Ruby: a.gcd(b)
来源：http://qno.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nkq.cheryme.top

[N06] 判断回文字符串
来源：http://yjv.sxryk.cn

Py:   s == s[::-1]
来源：http://lbo.mhx1999.top

PHP:  $s === strrev($s);
来源：http://wkk.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://uba.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://kjd.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zyb.yj20258888.top

Go:   // 双指针从两端比较
来源：http://ohd.zhengqikj.top

Ruby: s == s.reverse
来源：http://riq.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://smd.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://oub.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vpc.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hkw.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hkz.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://ivd.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://bwy.redwolf501.top

Go:   // 手写 map[int]int
来源：http://scj.tanke756.top

Ruby: // 手写 Hash
来源：http://crm.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://xlp.sufxvd.cn

[N08] 生成全排列
来源：http://qup.yongpay.top

Py:   itertools.permutations(arr)
来源：http://emd.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://esz.cucudq.cn

JS:   // 手写回溯递归
来源：http://igg.gzhubu.top

TS:   // 手写回溯递归
来源：http://mnu.sysykeji.top

Java: // 手写回溯递归
来源：http://iys.haohaochexian.top

Go:   // 手写回溯递归
来源：http://ngd.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://ezr.cqqwz.cn

C#:   // 手写回溯递归
来源：http://mpc.hammf.cn

[N09] 栈与队列
来源：http://vdk.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://edq.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gpt.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wqt.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xml.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nqb.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vwv.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wkn.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gve.tianlin.xyz

[N10] 链表节点定义
来源：http://xrb.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rqh.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eyj.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rkz.yj202588.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gcc.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://qtt.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://aoy.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mnd.yj20258.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cdb.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://zxq.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://emb.cashguo.top

PHP:  // 手写递归函数
来源：http://twg.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zek.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fqm.birdmap.top

Java: // 手写递归
来源：http://ygj.feifeiyinyue.top

Go:   // 手写递归
来源：http://okh.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ity.yj202588.top

C#:   // 手写递归
来源：http://vbi.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mll.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tyx.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hvr.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://syr.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kkk.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wwl.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zaz.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qft.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xjl.yj202588.top

================================================================================
来源：http://xhq.yuanzhike.top

O. 并发与异步
来源：http://aie.daxiang520.top

================================================================================
来源：http://ktx.yuanzhike.top

[O01] 启动一个线程
来源：http://ifu.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ffq.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ptp.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yfp.ctjpmb.com

TS:   // 同 JS
来源：http://apr.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://cwn.0kj1m.cn

Go:   go f()
来源：http://pet.nwbrower.top

Ruby: Thread.new { f }
来源：http://dgm.fzhhl.top

C#:   Task.Run(() => F());
来源：http://zue.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://hjk.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xqf.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jrz.ywan-chungtsiang.top

JS:   // worker_threads 线程池
来源：http://sme.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://ujf.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wfd.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aei.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iyf.xziqi.cn


<!-- 参考信息 -->