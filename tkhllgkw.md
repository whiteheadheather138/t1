代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fkf.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://jho.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mzl.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lse.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bzr.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hts.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kyo.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ejw.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://vtp.yj20258888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://izi.epnwcf.com

[K04] 读取 JSON 文件
来源：http://atr.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://whc.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sth.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xvl.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rfj.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ivr.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bxi.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rec.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kls.xinyue.icu

[K05] 深拷贝对象
来源：http://vps.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://igy.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://kol.fengsongda.top

JS:   structuredClone(obj)
来源：http://mav.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://rzv.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ddf.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iiv.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hgx.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://aor.tanke756.top

[K06] 解析 URL 查询串
来源：http://iis.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oke.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tef.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qwe.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gsr.jqgfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jnx.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://drh.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wvu.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aqu.xylfe.cn

[K07] 进制转换
来源：http://nna.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pbi.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pij.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://btf.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nem.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eoi.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vch.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fcz.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lec.jinyuanbaomall.cn

[K08] 二进制序列化（非 JSON）
来源：http://nsk.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://rbd.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://pli.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://owe.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://dni.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ncs.shangyingyoupin.top

Go:   encoding/gob
来源：http://rrj.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://kjh.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://svn.zhoulong.xyz

================================================================================
来源：http://bkn.zhoulong.xyz

L. 网络请求
来源：http://aax.yonumen.top

================================================================================
来源：http://hfj.nanxinkj.top

[L01] 发送 GET 请求
来源：http://cgu.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rfr.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dij.pengpengdd.cyou

JS:   await fetch(url)
来源：http://ajg.hammf.cn

TS:   await fetch(url)
来源：http://cjg.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ust.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://ssn.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xug.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xsx.yuxming.cn

[L02] 发送 POST JSON
来源：http://cnl.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://tdz.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://okn.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kww.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pbj.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cvk.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uzv.nwbrower.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wlu.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sox.xinyue.icu

[L03] 设置自定义请求头
来源：http://jrw.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cda.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://atz.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zgy.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ham.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yli.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yla.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://omt.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://suz.xuetiantiany.cn

[L04] 设置超时
来源：http://gmo.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://wis.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mzf.gaohongyu789.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uxt.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xtg.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lvn.daria6918.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sjy.smart0.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mnk.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tgs.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://wri.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qlr.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iit.hywenlv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mvh.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ovh.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yxc.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hvk.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pdj.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kxj.cheryme.top

[L06] 解析响应为 JSON
来源：http://idc.guannengcc.top

Py:   resp.json()
来源：http://yrn.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://lsj.tarul.cn

JS:   await resp.json()
来源：http://yjy.hfpthk.cn

TS:   await resp.json()
来源：http://mcd.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hpa.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://etb.uphjek.com

Ruby: JSON.parse(resp.body)
来源：http://xfq.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xmk.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://fik.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nse.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dbu.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://egs.316326.xyz

TS:   resp.ok;  resp.status
来源：http://bbz.yueranfly.top

Java: resp.statusCode()
来源：http://epz.sweek.top

Go:   resp.StatusCode
来源：http://hgq.jqgfzy.top

Ruby: resp.code.to_i
来源：http://iim.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://pim.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://shq.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ldv.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://pln.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mfm.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yte.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gjv.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://awa.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qew.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vmj.aibaodan.cn

================================================================================
来源：http://wmn.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://zra.quarkkingdee.top

================================================================================
来源：http://emi.fehbvm.com

[M01] 读取命令行参数
来源：http://gnp.redwolf501.top

Py:   sys.argv[1:]
来源：http://mjy.yj20258888.top

PHP:  $argv;  $argc;
来源：http://tzc.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://ppb.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://zdy.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://smz.jyoumei.cn

Go:   os.Args[1:]
来源：http://rrl.cdnleiting.top

Ruby: ARGV
来源：http://pcp.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://ndo.aizwys.cn

[M02] 读取环境变量
来源：http://pmo.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://mmk.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fyh.hfpthk.cn

JS:   process.env.HOME
来源：http://gkd.sxryk.cn

TS:   process.env.HOME
来源：http://qyg.fengsongda.top

Java: System.getenv("HOME")
来源：http://kix.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nzl.yuxming.cn

Ruby: ENV["HOME"]
来源：http://wyb.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vxb.cashguo.top

[M03] 执行外部命令
来源：http://fdu.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zfr.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://syq.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ozn.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gvw.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jcz.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dqe.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://bzf.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://iej.sysykeji.top

[M04] 获取当前工作目录
来源：http://afx.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://ckt.pycfn.com

PHP:  getcwd();
来源：http://won.epnwcf.com

JS:   process.cwd()
来源：http://rpg.hesvh.cn

TS:   process.cwd()
来源：http://aua.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://bvt.yj202588.top

Go:   os.Getwd()
来源：http://inz.0kj1m.cn

Ruby: Dir.pwd
来源：http://jvm.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://mpa.pengpengdd.cyou

[M05] 设置退出码
来源：http://mkz.zhixingplan.top

Py:   sys.exit(1)
来源：http://gpr.jyoumei.cn

PHP:  exit(1);
来源：http://ajj.nanxuanxn.top

JS:   process.exit(1)
来源：http://qge.52xcode.cn

TS:   process.exit(1)
来源：http://jqj.daxiang520.top

Java: System.exit(1)
来源：http://tvw.ctjpmb.com

Go:   os.Exit(1)
来源：http://qik.jlsjyb.cn

Ruby: exit 1
来源：http://asn.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gxe.hfpthk.cn

[M06] 向标准错误输出
来源：http://xmk.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://uba.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://sih.guowangkeji.top

JS:   console.error("err")
来源：http://ufr.chenlongwang.top

TS:   console.error("err")
来源：http://uhy.kuanghao11.cn

Java: System.err.println("err")
来源：http://gpb.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wzp.zhijiandao.cn

Ruby: warn "err"
来源：http://gma.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://qtk.xinyue.icu

[M07] 判断是否为主入口
来源：http://mum.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://mhz.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://igo.jiagoushi.top

JS:   require.main === module
来源：http://hnw.aibaodan.cn

TS:   require.main === module
来源：http://gio.dianchejie.cn

Java: public static void main(String[] args)
来源：http://svh.sweek.top

Go:   func main()
来源：http://fsb.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eke.yj20258.top

C#:   static void Main(string[] args)
来源：http://ezi.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://rww.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://srr.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://eik.andypj.xyz

JS:   process.platform;  process.version
来源：http://wib.xziqi.cn

TS:   process.platform;  process.version
来源：http://cbj.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pzo.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://icg.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mdy.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qbm.xziqi.cn

================================================================================
来源：http://xuc.andypj.xyz

N. 数据结构与算法
来源：http://him.ywan-chungtsiang.top

================================================================================
来源：http://uvg.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://sym.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jcf.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gui.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ruc.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jic.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aaq.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://idb.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jqx.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://wdk.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://cym.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://lzj.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bnq.epnwcf.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ydp.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ehd.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uot.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://lai.hnxiangtu.top

Ruby: arr.sort
来源：http://iqm.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hss.meibo888.top

[N03] 快速排序（分治示例）
来源：http://rlh.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dbg.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://roh.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bwq.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gbb.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zxl.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ssd.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uia.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://avm.gotoacloud.top

[N04] 斐波那契数列
来源：http://kpf.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hdc.xuanzx.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://njj.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ovh.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sar.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vsl.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wna.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qky.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uhj.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://blu.fehbvm.com

Py:   math.gcd(a, b)
来源：http://rrt.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yir.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://acu.cqqwz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://peh.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aut.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lmx.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://izw.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jvg.9152youxi.cn

[N06] 判断回文字符串
来源：http://ulv.cdnleiting.top

Py:   s == s[::-1]
来源：http://wqy.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://dbd.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://kbn.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://tew.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yzv.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://gvh.yfazqb.com

Ruby: s == s.reverse
来源：http://ixd.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cpt.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://rxn.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baj.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rul.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oob.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://zgx.bbcook.cn

Java: // 手写 HashMap
来源：http://qzi.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://mfn.zhengqikj.top

Ruby: // 手写 Hash
来源：http://wrg.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yml.mhx1999.top

[N08] 生成全排列
来源：http://niq.cheryme.top

Py:   itertools.permutations(arr)
来源：http://wdt.dashuyun.cn

PHP:  // 手写递归交换
来源：http://ffm.fzhhl.top

JS:   // 手写回溯递归
来源：http://dio.52xcode.cn

TS:   // 手写回溯递归
来源：http://fmt.tanke756.top

Java: // 手写回溯递归
来源：http://emh.gzhubu.top

Go:   // 手写回溯递归
来源：http://zpm.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://mbz.iojbl.cn

C#:   // 手写回溯递归
来源：http://jms.0kj1m.cn

[N09] 栈与队列
来源：http://iqs.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ldt.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eku.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lar.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tsz.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vsg.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cka.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hyb.gotoacloud.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://esn.zhiwuduotai.top

[N10] 链表节点定义
来源：http://tgy.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pkk.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ksg.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uai.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dhy.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://xrv.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mdk.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vnb.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hbj.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://ylo.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oiw.chenzaomai.com


<!-- 参考信息 -->