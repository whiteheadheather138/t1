代发 wailian999

[K02] JSON 字符串转对象
来源：http://frs.zhengqikj.top

Py:   json.loads(s)
来源：http://wkl.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tcd.shanyushiyangkeji.top

JS:   JSON.parse(s)
来源：http://bbp.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://wbn.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lsg.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://cbe.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://ylj.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ysj.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://hiw.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ecx.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://otz.yj20258.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pfr.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://veh.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://anj.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://npb.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://goa.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zoj.shuidangran.top

[K04] 读取 JSON 文件
来源：http://xzu.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fhk.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://avv.tarul.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvx.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jsr.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mzs.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://usg.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iyv.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://axy.zhengqikj.top

[K05] 深拷贝对象
来源：http://zeh.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://wzx.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://bjy.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://itg.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://jjg.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lam.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sgm.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uua.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lbm.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://ryi.xziqi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://idi.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bel.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fmq.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bkc.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lut.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lhf.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tus.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yuz.mhx1999.top

[K07] 进制转换
来源：http://vrh.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cyn.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://khc.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rud.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cyr.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zwv.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fbw.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://chu.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://seh.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://zyd.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://eqh.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ava.haohaochexian.top

JS:   v8.serialize(obj)        // Node
来源：http://pys.yvedp.cn

TS:   v8.serialize(obj)        // Node
来源：http://ivm.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lfi.hnqzz.top

Go:   encoding/gob
来源：http://lnk.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://ymf.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vlf.fktsv.cn

================================================================================
来源：http://jij.zhiwuduotai.top

L. 网络请求
来源：http://vhe.jinqigfzy.top

================================================================================
来源：http://mgv.yfazqb.com

[L01] 发送 GET 请求
来源：http://xtq.ivvv.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gkb.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aqs.sysykeji.top

JS:   await fetch(url)
来源：http://jqp.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://ple.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dxh.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://ouh.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jxw.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gxs.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://cin.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://dzo.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rtz.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kkz.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bfp.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sbg.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://drx.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nhc.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://myc.9152youxi.cn

[L03] 设置自定义请求头
来源：http://pgl.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://amc.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ccp.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iwn.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sia.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pzf.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://orp.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://upk.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wza.cdnleiting.top

[L04] 设置超时
来源：http://ymm.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://bgn.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hvu.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vuk.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swe.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ojc.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jzn.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://log.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wok.wangdashe.top

[L05] 上传文件（multipart）
来源：http://fvu.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gpo.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jie.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lxb.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rbs.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bla.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gzf.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wdz.wangshuangyany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qqo.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://oxp.shanyushiyangtech.top

Py:   resp.json()
来源：http://vot.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://yyb.zdbjq.cn

JS:   await resp.json()
来源：http://fdk.tianlin.xyz

TS:   await resp.json()
来源：http://imd.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://etz.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vmk.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://zav.shangyingyoupin.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iln.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://pic.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rhz.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dtk.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://byc.cashguo.top

TS:   resp.ok;  resp.status
来源：http://xas.sweek.top

Java: resp.statusCode()
来源：http://glk.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://hxu.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://gwr.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://mav.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://zyy.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qba.gaohongyu789.top

PHP:  curl_multi_init() 系列
来源：http://gzb.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://muz.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lal.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nof.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qxy.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nko.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fbl.bjfxy.top

================================================================================
来源：http://esq.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://ulx.zhaomingkeji.xyz

================================================================================
来源：http://sis.xuanzx.com

[M01] 读取命令行参数
来源：http://nuo.epnwcf.com

Py:   sys.argv[1:]
来源：http://xcg.xinyue.icu

PHP:  $argv;  $argc;
来源：http://bjr.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://ljh.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://wop.ctjpmb.com

Java: args 数组（main 方法参数）
来源：http://jsc.ppjwa.cn

Go:   os.Args[1:]
来源：http://cfr.yueranfly.top

Ruby: ARGV
来源：http://xlo.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://hms.yfazqb.com

[M02] 读取环境变量
来源：http://cxc.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://dex.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ban.jqgfzy.top

JS:   process.env.HOME
来源：http://okf.jqgufenzy.top

TS:   process.env.HOME
来源：http://ruh.jinqigufen.top

Java: System.getenv("HOME")
来源：http://tgk.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ezb.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://wsy.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uag.jiagoushi.top

[M03] 执行外部命令
来源：http://phm.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cnr.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eho.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xza.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bkj.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aco.hnqzz.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jnf.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ioi.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://zxe.yfazqb.com

[M04] 获取当前工作目录
来源：http://fnv.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://nyk.pycfn.com

PHP:  getcwd();
来源：http://kwx.ydjk.org.cn

JS:   process.cwd()
来源：http://alg.tianlin.xyz

TS:   process.cwd()
来源：http://pvs.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://lsz.gzhubu.top

Go:   os.Getwd()
来源：http://pao.cdnleiting.top

Ruby: Dir.pwd
来源：http://jpl.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://vht.tanke756.top

[M05] 设置退出码
来源：http://xjs.jinqigfzy.top

Py:   sys.exit(1)
来源：http://qlk.iojbl.cn

PHP:  exit(1);
来源：http://pop.birdmap.top

JS:   process.exit(1)
来源：http://qaf.52xcode.cn

TS:   process.exit(1)
来源：http://sxi.yueranfly.top

Java: System.exit(1)
来源：http://yjw.vehdjk.com

Go:   os.Exit(1)
来源：http://vob.ppjwa.cn

Ruby: exit 1
来源：http://xrl.9152youxi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://upf.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://aja.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://npd.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://brt.zhixingplan.top

JS:   console.error("err")
来源：http://orx.vehdjk.com

TS:   console.error("err")
来源：http://nby.zhixingplan.top

Java: System.err.println("err")
来源：http://jnf.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vdo.jianghu66.top

Ruby: warn "err"
来源：http://dra.tarul.cn

C#:   Console.Error.WriteLine("err")
来源：http://lfn.cashguo.top

[M07] 判断是否为主入口
来源：http://mvr.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://xvy.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sau.shanyushiyangkeji.top

JS:   require.main === module
来源：http://int.cashguo.top

TS:   require.main === module
来源：http://usu.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://nej.cdnleiting.top

Go:   func main()
来源：http://eoy.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bhd.fktsv.cn

C#:   static void Main(string[] args)
来源：http://cgt.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://wxf.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://ixy.epnwcf.com

PHP:  PHP_OS;  phpversion();
来源：http://zek.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://uhi.xinyue.icu

TS:   process.platform;  process.version
来源：http://mzy.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ena.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://irn.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iwj.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gqt.yuxming.cn

================================================================================
来源：http://qol.haohaochexian.top

N. 数据结构与算法
来源：http://jbc.hnxiangtu.top

================================================================================
来源：http://yde.feifeiyinyue.top

[N01] 二分查找（有序数组）
来源：http://rid.sxryk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jso.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zlm.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ioo.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://raw.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://eeg.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://tbq.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://tpv.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uns.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://qnw.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://snp.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fyh.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ijh.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://anb.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jri.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://utz.tanke756.top

Ruby: arr.sort
来源：http://dtm.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gsl.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://bjr.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zxe.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://bwd.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mdl.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://spi.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jda.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://frw.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mfe.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://xvw.hysaishi.cn

[N04] 斐波那契数列
来源：http://plz.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xov.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://noq.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hxy.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uez.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mdk.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xkh.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gmp.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kxp.ivvv.top

[N05] 最大公约数
来源：http://zdt.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://jns.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pjq.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mjq.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hvm.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://err.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lhn.daxiang520.top

Ruby: a.gcd(b)
来源：http://mfr.nwbrower.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yvf.cucudq.cn

[N06] 判断回文字符串
来源：http://ukx.gaohongyu789.top

Py:   s == s[::-1]
来源：http://cnw.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://ckb.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://qax.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://cfj.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bqy.cheryme.top

Go:   // 双指针从两端比较
来源：http://hkl.ydzc1.top

Ruby: s == s.reverse
来源：http://sxj.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ibt.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://mpg.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qak.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rge.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://fyi.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://uje.jqgfzy.top

Java: // 手写 HashMap
来源：http://ley.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://nmn.ydzc1.top

Ruby: // 手写 Hash
来源：http://xaj.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://ctf.zdqjudy.top

[N08] 生成全排列
来源：http://ljq.xingfuxueyuan.xyz

Py:   itertools.permutations(arr)
来源：http://joy.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://sxg.daria6918.cn

JS:   // 手写回溯递归
来源：http://jqb.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://qjh.andypj.xyz

Java: // 手写回溯递归
来源：http://tqb.bbcook.cn

Go:   // 手写回溯递归
来源：http://pqi.daxiang520.top

Ruby: arr.permutation.to_a
来源：http://kik.tarul.cn

C#:   // 手写回溯递归
来源：http://xyl.sweek.top

[N09] 栈与队列
来源：http://tag.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wdi.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bqg.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hsh.sysykeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fem.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jix.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://npt.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vhz.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://byy.vqdsnc.cn

[N10] 链表节点定义
来源：http://xde.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aqe.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://qhz.ybcxt.top


<!-- 参考信息 -->