代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://rse.xuanzx.com

PHP:  unserialize(serialize($obj));
来源：http://xvx.aibaodan.cn

JS:   structuredClone(obj)
来源：http://ijn.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://fek.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://oxj.zhengqikj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jnh.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ori.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iyt.fengsongda.top

[K06] 解析 URL 查询串
来源：http://lws.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nud.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vjn.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zjd.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://njn.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pwi.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://btm.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yoz.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pjb.jlsjyb.cn

[K07] 进制转换
来源：http://iaa.yuxming.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yee.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://acy.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ydv.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qgu.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lci.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nql.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dpo.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rdm.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://geo.sjlbkw.cn

Py:   pickle.dumps(obj)
来源：http://nik.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kqc.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://nra.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://vwh.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://efk.jinghuilouyu.cn

Go:   encoding/gob
来源：http://gnw.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://vmm.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oeg.cashguo.top

================================================================================
来源：http://mun.yangfankeji.com

L. 网络请求
来源：http://rri.jyoumei.cn

================================================================================
来源：http://hfs.meibo888.top

[L01] 发送 GET 请求
来源：http://lgm.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://twn.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://igd.zhoulong.xyz

JS:   await fetch(url)
来源：http://tay.yfazqb.com

TS:   await fetch(url)
来源：http://jak.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vqd.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://mvy.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zot.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uyq.xuetiantiany.cn

[L02] 发送 POST JSON
来源：http://dkl.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://uqd.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jwn.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://igf.quarkkingdee.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yjq.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://enq.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tvl.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mva.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pof.fengsongda.top

[L03] 设置自定义请求头
来源：http://wsy.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nze.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wnc.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://akz.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jxl.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fqf.svipenyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pxj.vqdsnc.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vdr.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uve.hfpthk.cn

[L04] 设置超时
来源：http://knf.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://nbj.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://par.snrcjt.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://enu.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzx.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xki.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wqo.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kgu.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vtj.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://umv.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cwe.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kir.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jbc.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nyp.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://llm.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cnw.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xri.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jci.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://ktb.zhiwuduotai.top

Py:   resp.json()
来源：http://pfw.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://ool.yj20258.top

JS:   await resp.json()
来源：http://kbi.hfpthk.cn

TS:   await resp.json()
来源：http://eqz.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lpy.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zqk.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://hrb.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wmn.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://wvg.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://clo.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ymt.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://zyp.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://rxx.ybcxt.top

Java: resp.statusCode()
来源：http://tsj.fktsv.cn

Go:   resp.StatusCode
来源：http://urf.svipenyu.cn

Ruby: resp.code.to_i
来源：http://bzy.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://ocv.c1oappe.top

[L08] 并发请求多个地址
来源：http://juc.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gcv.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://rhz.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mqs.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mnl.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ngk.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pxi.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tpa.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dlo.chenjidiqi.icu

================================================================================
来源：http://lpj.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://cnl.chenjidiqi.icu

================================================================================
来源：http://bkb.birdmap.top

[M01] 读取命令行参数
来源：http://hga.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://bqq.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://uxt.tian-w.cn

JS:   process.argv.slice(2)
来源：http://xsr.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://ngs.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://qsz.tanke756.top

Go:   os.Args[1:]
来源：http://gst.hcnkem.com

Ruby: ARGV
来源：http://swr.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://yuf.vqdsnc.cn

[M02] 读取环境变量
来源：http://bjr.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://fie.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://joj.fktsv.cn

JS:   process.env.HOME
来源：http://slw.sxryk.cn

TS:   process.env.HOME
来源：http://ifw.sysykeji.top

Java: System.getenv("HOME")
来源：http://yez.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rdk.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://acp.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://maj.fzhhl.top

[M03] 执行外部命令
来源：http://fxd.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xda.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://veu.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ekq.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://xek.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tmj.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zly.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://nrq.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://hvr.sufxvd.cn

[M04] 获取当前工作目录
来源：http://zhz.snrcjt.cn

Py:   os.getcwd()
来源：http://ljk.gzhubu.top

PHP:  getcwd();
来源：http://nam.havefunace.top

JS:   process.cwd()
来源：http://umk.yongpay.top

TS:   process.cwd()
来源：http://deg.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://but.wangdashe.top

Go:   os.Getwd()
来源：http://cxq.fktsv.cn

Ruby: Dir.pwd
来源：http://gwi.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://uqy.cdnleiting.top

[M05] 设置退出码
来源：http://wts.gogol.net.cn

Py:   sys.exit(1)
来源：http://uwx.yuanzhike.top

PHP:  exit(1);
来源：http://wqr.ppjwa.cn

JS:   process.exit(1)
来源：http://fok.ydzc1.top

TS:   process.exit(1)
来源：http://uri.zdbjq.cn

Java: System.exit(1)
来源：http://hvo.smart0.xyz

Go:   os.Exit(1)
来源：http://mwv.cqqwz.cn

Ruby: exit 1
来源：http://sao.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pyg.hammf.cn

[M06] 向标准错误输出
来源：http://fse.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://elr.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yrs.guannengcc.top

JS:   console.error("err")
来源：http://upd.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://doz.feifeiyinyue.top

Java: System.err.println("err")
来源：http://qga.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qwq.xinyue.icu

Ruby: warn "err"
来源：http://qvp.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://tei.aizwys.cn

[M07] 判断是否为主入口
来源：http://jtr.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://xjb.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ead.jianghu66.top

JS:   require.main === module
来源：http://dfo.chenlongwang.top

TS:   require.main === module
来源：http://lod.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://hsq.wangdashe.top

Go:   func main()
来源：http://joq.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ikc.sxryk.cn

C#:   static void Main(string[] args)
来源：http://dal.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://mmj.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://viz.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://jko.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://hka.nanxinkj.top

TS:   process.platform;  process.version
来源：http://obq.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pgo.sysykeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mvj.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://azr.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ofz.yvedp.cn

================================================================================
来源：http://ptm.jlsjyb.cn

N. 数据结构与算法
来源：http://xmt.daria6918.cn

================================================================================
来源：http://xta.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://cmo.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yog.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tzk.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zpk.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vaf.daxiang520.top

Java: Arrays.binarySearch(arr, x)
来源：http://hxq.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://otf.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aps.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://ndc.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://itt.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://scu.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aap.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://noc.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://obm.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mst.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://kki.zhoulong.xyz

Ruby: arr.sort
来源：http://taw.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://whu.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://mft.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rlv.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://xdy.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ahz.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zyh.zhengqikj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dzy.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://efq.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wgk.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zlj.shuidangran.top

[N04] 斐波那契数列
来源：http://bnh.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cjh.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ysb.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ojh.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qfc.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rkt.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vtx.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pij.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nag.0kj1m.cn

[N05] 最大公约数
来源：http://aky.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://qvf.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gjq.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lcy.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xxj.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pzi.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zqh.vehdjk.com

Ruby: a.gcd(b)
来源：http://eey.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eko.yj20258.top

[N06] 判断回文字符串
来源：http://nhv.ybcxt.top

Py:   s == s[::-1]
来源：http://rtp.hcnkem.com

PHP:  $s === strrev($s);
来源：http://soa.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://wey.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://gng.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tns.birdmap.top

Go:   // 双指针从两端比较
来源：http://lqn.316326.xyz

Ruby: s == s.reverse
来源：http://hlj.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yuv.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://nsa.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://omh.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jug.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gip.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://cve.chenzaomai.com

Java: // 手写 HashMap
来源：http://qmu.hcnkem.com

Go:   // 手写 map[int]int
来源：http://zxf.zhijiandao.cn

Ruby: // 手写 Hash
来源：http://ngo.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://ivc.xylfe.cn

[N08] 生成全排列
来源：http://aay.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://fnn.yuxming.cn

PHP:  // 手写递归交换
来源：http://ecz.yuxming.cn

JS:   // 手写回溯递归
来源：http://iys.yuxming.cn

TS:   // 手写回溯递归
来源：http://zmw.mhx1999.top

Java: // 手写回溯递归
来源：http://doo.mhx1999.top

Go:   // 手写回溯递归
来源：http://wfn.hammf.cn

Ruby: arr.permutation.to_a
来源：http://qes.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://ckp.mhx1999.top

[N09] 栈与队列
来源：http://mjz.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vlf.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fsh.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mvi.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hpr.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lsa.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aya.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iht.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gdc.tian-w.cn

[N10] 链表节点定义
来源：http://fpy.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jhc.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://swl.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dsl.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cbb.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://iic.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://fzl.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wte.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://exk.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://yjm.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ueg.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://aby.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cwa.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jrb.hnxiangtu.top

Java: // 手写递归
来源：http://ihj.yonumen.top

Go:   // 手写递归
来源：http://bpb.tian-w.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mwv.cqqwz.cn

C#:   // 手写递归
来源：http://mjv.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yzg.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jdd.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pji.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nmn.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xjj.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kad.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lcd.zdbjq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nkc.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fec.daria6918.cn

================================================================================
来源：http://uzd.hywenlv.cn

O. 并发与异步
来源：http://kqw.hongshengwenyu.top

================================================================================
来源：http://pyv.tianlin.xyz

[O01] 启动一个线程
来源：http://gye.bjfxy.top


<!-- 参考信息 -->