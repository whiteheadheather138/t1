代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://hdg.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ikn.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dct.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rcg.xylfe.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fgo.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bbf.fehbvm.com

[K04] 读取 JSON 文件
来源：http://tvs.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pkg.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rmn.tarul.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vah.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xny.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xvg.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xzc.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jyg.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://veb.svipenyu.cn

[K05] 深拷贝对象
来源：http://bpw.pycfn.com

Py:   copy.deepcopy(obj)
来源：http://zne.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://gvt.dianchejie.cn

JS:   structuredClone(obj)
来源：http://gvd.hfpthk.cn

TS:   structuredClone(obj)
来源：http://sgv.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://shl.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ytm.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tug.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ayh.andypj.xyz

[K06] 解析 URL 查询串
来源：http://vhn.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kwy.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kir.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pip.birdmap.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://usv.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tqr.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lop.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wbs.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hof.hcnkem.com

[K07] 进制转换
来源：http://llz.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ico.zdbjq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cbx.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zsj.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dvd.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wft.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cyq.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iiv.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dut.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://sds.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://wub.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sjs.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://gge.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://qxo.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kpt.hysaishi.cn

Go:   encoding/gob
来源：http://uao.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://cca.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ros.pycfn.com

================================================================================
来源：http://vjk.haohaochexian.top

L. 网络请求
来源：http://gin.jyoumei.cn

================================================================================
来源：http://ysx.ctjpmb.com

[L01] 发送 GET 请求
来源：http://yla.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://urx.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jht.andypj.xyz

JS:   await fetch(url)
来源：http://sgr.yongpay.top

TS:   await fetch(url)
来源：http://tni.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qlp.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://smz.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://vzn.jinyuanbaomall.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ome.yongpay.top

[L02] 发送 POST JSON
来源：http://bwu.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://uyt.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://skc.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kbc.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ohc.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qid.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nam.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gzn.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mio.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://obe.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vtu.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vvh.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpm.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rfh.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ciu.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sje.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tab.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nku.0kj1m.cn

[L04] 设置超时
来源：http://qaq.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://vun.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ovh.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dbp.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://noc.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ufo.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mfe.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vjz.ydzc1.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ooy.yueranfly.top

[L05] 上传文件（multipart）
来源：http://jxp.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qax.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mxr.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yyo.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ici.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gzg.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vgt.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://twy.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pte.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://fer.yongpay.top

Py:   resp.json()
来源：http://smk.fanxiaobao.xyz

PHP:  json_decode($body, true);
来源：http://beu.ydzc1.top

JS:   await resp.json()
来源：http://hvj.shzxlz.cn

TS:   await resp.json()
来源：http://dho.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rqz.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://usa.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://ads.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://grj.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://rxe.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pwd.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aaf.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://drj.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://ndo.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://xfi.tian-w.cn

Go:   resp.StatusCode
来源：http://oul.vehdjk.com

Ruby: resp.code.to_i
来源：http://tis.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://smf.gogol.net.cn

[L08] 并发请求多个地址
来源：http://jkd.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://def.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://rpl.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kyo.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pwx.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mge.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fcz.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://whx.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fgd.guannengcc.top

================================================================================
来源：http://dwp.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://oub.shanyushiyangkeji.top

================================================================================
来源：http://wwq.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://ozf.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://vxn.cucudq.cn

PHP:  $argv;  $argc;
来源：http://cvz.fktsv.cn

JS:   process.argv.slice(2)
来源：http://bnd.fzhhl.top

TS:   process.argv.slice(2)
来源：http://auv.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://vki.ydzc1.top

Go:   os.Args[1:]
来源：http://rgu.yvedp.cn

Ruby: ARGV
来源：http://crx.shanyushiyangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://jju.9152youxi.cn

[M02] 读取环境变量
来源：http://asg.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://qxe.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rfb.xuetiantiany.cn

JS:   process.env.HOME
来源：http://gjr.yfazqb.com

TS:   process.env.HOME
来源：http://lgs.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://ksl.yanxiufei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rzw.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://foc.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yus.fehbvm.com

[M03] 执行外部命令
来源：http://wqo.feifeiyinyue.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nfs.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://auh.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vda.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pkt.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fbi.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ued.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ptb.zhaomingkeji.xyz

C#:   Process.Start("ls", "-l");
来源：http://ezm.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://haa.yuanzhike.top

Py:   os.getcwd()
来源：http://rdy.redwolf501.top

PHP:  getcwd();
来源：http://zkd.chenzaomai.com

JS:   process.cwd()
来源：http://vfx.cucudq.cn

TS:   process.cwd()
来源：http://vkj.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://yno.cucudq.cn

Go:   os.Getwd()
来源：http://cul.guannengcc.top

Ruby: Dir.pwd
来源：http://eah.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://nzm.kuanghao11.cn

[M05] 设置退出码
来源：http://ive.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://obz.chenjidiqi.icu

PHP:  exit(1);
来源：http://kvy.hammf.cn

JS:   process.exit(1)
来源：http://pmh.hysaishi.cn

TS:   process.exit(1)
来源：http://wro.gzhubu.top

Java: System.exit(1)
来源：http://xlh.vqdsnc.cn

Go:   os.Exit(1)
来源：http://mpp.vehdjk.com

Ruby: exit 1
来源：http://fnk.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qqx.xinyue.icu

[M06] 向标准错误输出
来源：http://wjw.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://vgl.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kad.jinqigufen.top

JS:   console.error("err")
来源：http://ltz.jlsjyb.cn

TS:   console.error("err")
来源：http://tou.ehwqpu.com

Java: System.err.println("err")
来源：http://yqj.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nop.tianlin.xyz

Ruby: warn "err"
来源：http://lym.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://ujc.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://xxf.kuanghao11.cn

Py:   if __name__ == "__main__":
来源：http://yyr.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oez.yongpay.top

JS:   require.main === module
来源：http://yvx.ywan-chungtsiang.top

TS:   require.main === module
来源：http://xyr.dashuyun.cn

Java: public static void main(String[] args)
来源：http://vkn.shanyushiyangtech.top

Go:   func main()
来源：http://eir.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rnn.xinyue.icu

C#:   static void Main(string[] args)
来源：http://gzo.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://mns.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://hdo.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://wwv.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://xji.hnqzz.top

TS:   process.platform;  process.version
来源：http://khw.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gdt.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://otu.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://olt.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fgh.zhijiandao.cn

================================================================================
来源：http://emd.tarul.cn

N. 数据结构与算法
来源：http://jxl.zdqjudy.top

================================================================================
来源：http://ycd.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://gim.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://cqn.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://swq.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mzl.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fbw.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://pdv.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://phw.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gqs.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://got.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://ipc.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://hbm.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qww.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://pec.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gmb.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xnw.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://qhv.nanxuanxn.top

Ruby: arr.sort
来源：http://jti.zhijiandao.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cgj.daxiang520.top

[N03] 快速排序（分治示例）
来源：http://foy.zhiwuduotai.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iez.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://gnu.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ebk.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gii.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gtl.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xhl.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jrs.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jaq.hesvh.cn

[N04] 斐波那契数列
来源：http://uwn.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kzu.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lsh.dianchejie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://klx.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uit.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kui.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gox.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xvk.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cnu.cheryme.top

[N05] 最大公约数
来源：http://xuv.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://clj.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cdw.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ona.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://awz.yfazqb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uqw.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kym.c1oappe.top

Ruby: a.gcd(b)
来源：http://xos.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eey.hysaishi.cn

[N06] 判断回文字符串
来源：http://gtd.xziqi.cn

Py:   s == s[::-1]
来源：http://jbw.daria6918.cn

PHP:  $s === strrev($s);
来源：http://ams.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://cdt.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://rtd.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rnu.smart0.xyz

Go:   // 双指针从两端比较
来源：http://laa.epnwcf.com

Ruby: s == s.reverse
来源：http://ufx.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yqq.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://jfx.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://azf.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ewx.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ldr.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://lfi.chenzaomai.com

Java: // 手写 HashMap
来源：http://rdq.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://mgf.iojbl.cn

Ruby: // 手写 Hash
来源：http://nls.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://lqg.jqgufenzy.top

[N08] 生成全排列
来源：http://cbg.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://clk.snrcjt.cn

PHP:  // 手写递归交换
来源：http://ptk.dashuyun.cn

JS:   // 手写回溯递归
来源：http://qvk.jinqigufen.top

TS:   // 手写回溯递归
来源：http://fcp.tanke756.top

Java: // 手写回溯递归
来源：http://eiy.ybcxt.top

Go:   // 手写回溯递归
来源：http://zbj.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://hyz.dianchejie.cn

C#:   // 手写回溯递归
来源：http://gfo.havefunace.top

[N09] 栈与队列
来源：http://sug.iojbl.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jkr.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ffc.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bsr.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bkv.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://otd.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://miy.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rrz.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mqg.52xcode.cn

[N10] 链表节点定义
来源：http://ilp.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://are.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://azc.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hoa.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ihe.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://hir.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://lzs.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hvd.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://duo.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://wfl.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jjp.yuxming.cn

PHP:  // 手写递归函数
来源：http://rbh.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tod.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jvi.ybcxt.top

Java: // 手写递归
来源：http://spq.ybcxt.top


<!-- 参考信息 -->