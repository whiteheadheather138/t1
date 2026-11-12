代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://piu.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mce.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kpx.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ixj.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://svy.hongshengwenyu.top

[K07] 进制转换
来源：http://mdk.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://itt.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zvm.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://axi.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ubd.jinyuanbaomall.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uqr.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dbl.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mvy.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qtz.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://thd.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://uer.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xoj.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://wwt.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://sco.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hkv.ybcxt.top

Go:   encoding/gob
来源：http://vmn.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://uho.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xoy.fanxiaobao.xyz

================================================================================
来源：http://ngn.c1oappe.top

L. 网络请求
来源：http://yyh.nwbrower.top

================================================================================
来源：http://kkp.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://ggc.ehwqpu.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://udy.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wck.tarul.cn

JS:   await fetch(url)
来源：http://wqb.kuanghao11.cn

TS:   await fetch(url)
来源：http://lpe.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hks.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://pep.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://baa.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nlu.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://dip.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kob.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xos.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cld.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jgf.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xbk.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ret.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uhz.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ddz.yvedp.cn

[L03] 设置自定义请求头
来源：http://qkn.havefunace.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hpj.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vck.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wfb.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qca.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bdd.hammf.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://deg.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tvk.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rsg.iojbl.cn

[L04] 设置超时
来源：http://sna.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://tzl.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://enj.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jgd.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://agr.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jse.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yon.xingfuxueyuan.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pmp.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lim.xylfe.cn

[L05] 上传文件（multipart）
来源：http://mea.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bvt.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wzy.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oow.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://epf.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cmt.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vdc.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jfp.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jzg.yonumen.top

[L06] 解析响应为 JSON
来源：http://vjq.shzxlz.cn

Py:   resp.json()
来源：http://fsu.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://asq.vqdsnc.cn

JS:   await resp.json()
来源：http://jhd.shuidangran.top

TS:   await resp.json()
来源：http://bbf.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ayv.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ngh.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://ebx.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://avj.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://jli.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://idx.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vvo.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://fdl.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://tho.jqgufenzy.top

Java: resp.statusCode()
来源：http://woc.nanxuanxn.top

Go:   resp.StatusCode
来源：http://stx.ehwqpu.com

Ruby: resp.code.to_i
来源：http://mkq.tanke756.top

C#:   (int)resp.StatusCode
来源：http://hvi.xziqi.cn

[L08] 并发请求多个地址
来源：http://wmt.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vtb.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://gps.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ivt.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://azx.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pqw.tanke756.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pfs.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qyd.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pmy.shanyushiyangtech.top

================================================================================
来源：http://cbq.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://gte.yueranfly.top

================================================================================
来源：http://ujz.redwolf501.top

[M01] 读取命令行参数
来源：http://rkn.zycfv.cn

Py:   sys.argv[1:]
来源：http://chn.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://frk.cashguo.top

JS:   process.argv.slice(2)
来源：http://kuz.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://kjz.uphjek.com

Java: args 数组（main 方法参数）
来源：http://rlk.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://jxf.ybcxt.top

Ruby: ARGV
来源：http://fcg.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://kls.shanyushiyangtech.top

[M02] 读取环境变量
来源：http://zho.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://don.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qoy.snrcjt.cn

JS:   process.env.HOME
来源：http://ikc.epnwcf.com

TS:   process.env.HOME
来源：http://dxv.andypj.xyz

Java: System.getenv("HOME")
来源：http://iow.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zka.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://ytq.shanyushiyangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vsr.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://qmm.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tkv.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jdo.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ocb.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fhx.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mlb.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://osk.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://cor.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://lea.yonumen.top

[M04] 获取当前工作目录
来源：http://rnb.bbcook.cn

Py:   os.getcwd()
来源：http://wou.xuanzx.com

PHP:  getcwd();
来源：http://cdx.fanxiaobao.xyz

JS:   process.cwd()
来源：http://qjh.hammf.cn

TS:   process.cwd()
来源：http://lfm.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://kpx.zhongyouzk.top

Go:   os.Getwd()
来源：http://mzm.pycfn.com

Ruby: Dir.pwd
来源：http://yts.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://kni.quarkkingdee.top

[M05] 设置退出码
来源：http://usr.chenzaomai.com

Py:   sys.exit(1)
来源：http://ido.hfpthk.cn

PHP:  exit(1);
来源：http://bsg.gotoacloud.top

JS:   process.exit(1)
来源：http://wgr.dashuyun.cn

TS:   process.exit(1)
来源：http://dvz.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://yxw.hnqzz.top

Go:   os.Exit(1)
来源：http://hnb.zhijiandao.cn

Ruby: exit 1
来源：http://jhf.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pol.quarkkingdee.top

[M06] 向标准错误输出
来源：http://qef.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://zny.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tyf.nanxuanxn.top

JS:   console.error("err")
来源：http://acd.pengpengdd.cyou

TS:   console.error("err")
来源：http://pjr.andypj.xyz

Java: System.err.println("err")
来源：http://zck.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zsl.ydjk.org.cn

Ruby: warn "err"
来源：http://yhu.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://swe.zhengqikj.top

[M07] 判断是否为主入口
来源：http://qmw.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://heb.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mxh.ppjwa.cn

JS:   require.main === module
来源：http://khp.jqgfzy.top

TS:   require.main === module
来源：http://svf.guannengcc.top

Java: public static void main(String[] args)
来源：http://sgs.iojbl.cn

Go:   func main()
来源：http://nil.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sew.guowangkeji.top

C#:   static void Main(string[] args)
来源：http://bnm.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://fol.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://glt.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://xrq.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://obz.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://rpf.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iux.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://iyw.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mtj.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://jyn.jqgufenzy.top

================================================================================
来源：http://vup.hongshengwenyu.top

N. 数据结构与算法
来源：http://app.fengsongda.top

================================================================================
来源：http://vmx.yj20258.top

[N01] 二分查找（有序数组）
来源：http://yfn.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mzu.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ggm.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rry.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kcb.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://pvu.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://kdf.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vxo.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://iyg.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://jor.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://xcb.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fti.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://gcm.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://wta.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blu.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://yqy.svipenyu.cn

Ruby: arr.sort
来源：http://pod.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mft.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://xsi.zhixingplan.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jej.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://onp.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wkm.yonumen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wul.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://evj.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ldn.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ztp.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://xyz.bbcook.cn

[N04] 斐波那契数列
来源：http://zrc.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ysy.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fzl.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ock.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bcv.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cps.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ncs.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ubi.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fzr.xinyue.icu

[N05] 最大公约数
来源：http://meg.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://blm.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://unl.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://myw.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nhp.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kme.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://clu.ydzc1.top

Ruby: a.gcd(b)
来源：http://iaa.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rlb.birdmap.top

[N06] 判断回文字符串
来源：http://amz.ctjpmb.com

Py:   s == s[::-1]
来源：http://whs.0kj1m.cn

PHP:  $s === strrev($s);
来源：http://etp.havefunace.top

JS:   s === [...s].reverse().join("")
来源：http://dhc.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://whg.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ahf.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://ggb.xylfe.cn

Ruby: s == s.reverse
来源：http://yct.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iwa.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://wkl.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uvn.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nxp.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://cur.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://vna.sweek.top

Java: // 手写 HashMap
来源：http://tyg.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://mps.zhixingplan.top

Ruby: // 手写 Hash
来源：http://gat.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xqk.hfpthk.cn

[N08] 生成全排列
来源：http://qfh.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://jqd.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://whx.yj202588.top

JS:   // 手写回溯递归
来源：http://con.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://jhn.zhengqikj.top

Java: // 手写回溯递归
来源：http://rer.aizwys.cn

Go:   // 手写回溯递归
来源：http://bbc.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://bra.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://xvp.zdbjq.cn

[N09] 栈与队列
来源：http://ubj.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eqg.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://igo.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nbu.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sie.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://btc.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eqq.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hzk.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mmt.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://rnn.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jkx.nanxuanxn.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tkw.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bqb.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uso.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://iep.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://uon.hnqzz.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ufp.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://bgc.bbcook.cn

[N11] 二叉树中序遍历
来源：http://chg.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mxc.yuxming.cn

PHP:  // 手写递归函数
来源：http://aff.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mxo.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://laq.jianghu66.top

Java: // 手写递归
来源：http://iqb.mhx1999.top

Go:   // 手写递归
来源：http://pzu.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vrr.bjfxy.top

C#:   // 手写递归
来源：http://jtx.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cdv.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wwy.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tfr.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jxk.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jdr.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cri.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vpl.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://efg.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://poz.zhoulong.xyz

================================================================================
来源：http://lov.shangyingyoupin.top

O. 并发与异步
来源：http://yxo.bjfxy.top

================================================================================
来源：http://gkj.vehdjk.com

[O01] 启动一个线程
来源：http://orn.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ewf.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tdd.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cgg.chenjidiqi.icu

TS:   // 同 JS
来源：http://ovx.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://uzo.cashguo.top

Go:   go f()
来源：http://viz.tanke756.top

Ruby: Thread.new { f }
来源：http://jlc.fengsongda.top

C#:   Task.Run(() => F());
来源：http://pec.yueranfly.top

[O02] 使用线程池
来源：http://ogl.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ehp.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dws.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://skc.cashguo.top


<!-- 参考信息 -->