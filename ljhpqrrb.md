代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lgi.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jyb.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xrp.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://ibk.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://baj.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ngq.ivvv.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rvl.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://smv.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fsq.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dme.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vhs.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rwi.bbcook.cn

================================================================================
来源：http://qkd.tianlin.xyz

K. JSON 与序列化
来源：http://klx.chenzaomai.com

================================================================================
来源：http://qpf.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://zgr.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bki.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pxo.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://chd.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://bne.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://czo.birdmap.top

Go:   json.Marshal(obj)
来源：http://kmb.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://zno.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wdx.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://tpl.sxryk.cn

Py:   json.loads(s)
来源：http://ufp.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jpd.daxiang520.top

JS:   JSON.parse(s)
来源：http://yqy.yuanzhike.top

TS:   JSON.parse(s)
来源：http://ujr.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nsf.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://htw.sysykeji.top

Ruby: JSON.parse(s)
来源：http://qlm.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://igg.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://ome.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uik.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pkk.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rhn.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://epo.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hsc.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mcp.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://iox.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://htl.mhx1999.top

[K04] 读取 JSON 文件
来源：http://red.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ujd.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qpa.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://way.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xil.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tqk.dashuyun.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lsc.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://yel.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yqa.hnqzz.top

[K05] 深拷贝对象
来源：http://lij.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://dej.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://rkw.gzhubu.top

JS:   structuredClone(obj)
来源：http://tnp.snrcjt.cn

TS:   structuredClone(obj)
来源：http://ltd.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dcm.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nqb.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zvv.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://whk.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://jdt.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dyz.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rtn.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://boq.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://irt.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://psc.bbcook.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://enj.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nnv.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vbo.fanxiaobao.xyz

[K07] 进制转换
来源：http://xuz.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oog.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://goh.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://boi.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yjq.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jqj.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://agp.jyoumei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://thk.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fcg.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://ofe.epnwcf.com

Py:   pickle.dumps(obj)
来源：http://ono.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ewh.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://uxr.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://zge.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://osj.yuxming.cn

Go:   encoding/gob
来源：http://gww.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://bex.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ywr.svipenyu.cn

================================================================================
来源：http://dvl.iojbl.cn

L. 网络请求
来源：http://kiz.quarkkingdee.top

================================================================================
来源：http://fko.daxiang520.top

[L01] 发送 GET 请求
来源：http://smr.jinqigfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wrh.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xjl.mhx1999.top

JS:   await fetch(url)
来源：http://ioq.zhongyouzk.top

TS:   await fetch(url)
来源：http://pwn.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gqm.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://oen.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ojy.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://svg.hywenlv.cn

[L02] 发送 POST JSON
来源：http://pcg.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://ggx.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tft.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ajb.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dyj.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xyn.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xhq.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nsn.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dpm.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://thg.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://swy.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ode.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jyr.9152youxi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tyo.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kar.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pqc.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ekr.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yxn.jlsjyb.cn

[L04] 设置超时
来源：http://dkj.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://ayr.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jne.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dnf.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bhr.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xma.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ggh.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jme.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://csl.ydjk.org.cn

[L05] 上传文件（multipart）
来源：http://mxy.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lwg.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fxi.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lsi.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xsu.zdqjudy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qla.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://but.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zhs.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dgn.bbcook.cn

[L06] 解析响应为 JSON
来源：http://dzb.shanyushiyangkeji.top

Py:   resp.json()
来源：http://gog.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://tpw.yongpay.top

JS:   await resp.json()
来源：http://jjp.9152youxi.cn

TS:   await resp.json()
来源：http://fcs.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yiw.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pzb.hnxiangtu.top

Ruby: JSON.parse(resp.body)
来源：http://qsl.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://koa.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://iqb.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dcd.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zzz.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://vkn.guowangkeji.top

TS:   resp.ok;  resp.status
来源：http://ouh.316326.xyz

Java: resp.statusCode()
来源：http://ebb.vehdjk.com

Go:   resp.StatusCode
来源：http://hgd.mhx1999.top

Ruby: resp.code.to_i
来源：http://bja.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://nad.tarul.cn

[L08] 并发请求多个地址
来源：http://srg.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://swy.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://bis.vehdjk.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dnd.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://swq.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zgv.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nga.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ehb.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tqz.andypj.xyz

================================================================================
来源：http://mjm.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://uwy.quarkkingdee.top

================================================================================
来源：http://hdv.hywenlv.cn

[M01] 读取命令行参数
来源：http://bnr.sweek.top

Py:   sys.argv[1:]
来源：http://ere.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://stb.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://vqt.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://ovh.ctjpmb.com

Java: args 数组（main 方法参数）
来源：http://aiz.cqqwz.cn

Go:   os.Args[1:]
来源：http://trf.yanxiufei.cn

Ruby: ARGV
来源：http://ldi.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://rgj.daxiang520.top

[M02] 读取环境变量
来源：http://wsi.zhijiandao.cn

Py:   os.environ.get("HOME")
来源：http://sme.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://slr.jlsjyb.cn

JS:   process.env.HOME
来源：http://kko.shzxlz.cn

TS:   process.env.HOME
来源：http://wmw.hywenlv.cn

Java: System.getenv("HOME")
来源：http://eiu.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ben.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://gyd.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fht.gaohongyu789.top

[M03] 执行外部命令
来源：http://wef.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://csv.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tkp.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pjr.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://cpz.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lpb.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ceh.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://ies.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://rjo.ybcxt.top

[M04] 获取当前工作目录
来源：http://rcr.daria6918.cn

Py:   os.getcwd()
来源：http://ndm.haohaochexian.top

PHP:  getcwd();
来源：http://pco.ydzc1.top

JS:   process.cwd()
来源：http://goc.shangyingyoupin.top

TS:   process.cwd()
来源：http://cbd.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://rjs.shzxlz.cn

Go:   os.Getwd()
来源：http://ofb.fengsongda.top

Ruby: Dir.pwd
来源：http://ayn.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://ezs.ybcxt.top

[M05] 设置退出码
来源：http://fqc.hysaishi.cn

Py:   sys.exit(1)
来源：http://acz.xuetiantiany.cn

PHP:  exit(1);
来源：http://ppm.tianlin.xyz

JS:   process.exit(1)
来源：http://baq.redwolf501.top

TS:   process.exit(1)
来源：http://cta.shzxlz.cn

Java: System.exit(1)
来源：http://nhe.xinyue.icu

Go:   os.Exit(1)
来源：http://btv.yuxming.cn

Ruby: exit 1
来源：http://uwe.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uzn.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://jqp.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://clt.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rbj.cheryme.top

JS:   console.error("err")
来源：http://zhl.hnqzz.top

TS:   console.error("err")
来源：http://bkw.zdqjudy.top

Java: System.err.println("err")
来源：http://lln.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://syc.zdqjudy.top

Ruby: warn "err"
来源：http://hws.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://mls.jianghu66.top

[M07] 判断是否为主入口
来源：http://grf.yj20258.top

Py:   if __name__ == "__main__":
来源：http://jpg.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://quy.hfpthk.cn

JS:   require.main === module
来源：http://vrg.hesvh.cn

TS:   require.main === module
来源：http://mjn.fzhhl.top

Java: public static void main(String[] args)
来源：http://jkr.jiagoushi.top

Go:   func main()
来源：http://dup.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xap.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://krk.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://ith.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://igd.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://eqn.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://mbt.xziqi.cn

TS:   process.platform;  process.version
来源：http://qfy.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cvx.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rnd.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qir.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wzi.pycfn.com

================================================================================
来源：http://mwz.pengpengdd.cyou

N. 数据结构与算法
来源：http://bqs.xuetiantiany.cn

================================================================================
来源：http://iox.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://hhp.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://ict.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xty.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://swi.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qjj.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://rzl.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://mdt.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tqo.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://ikd.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://scl.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://upj.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sot.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://num.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xrw.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tbc.bbcook.cn

Go:   slices.Sort(arr)
来源：http://suv.52xcode.cn

Ruby: arr.sort
来源：http://uum.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kcn.zhixingplan.top

[N03] 快速排序（分治示例）
来源：http://liw.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xoc.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://kjg.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bty.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsb.andypj.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://deu.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ziz.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bwf.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zpm.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://zki.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kdi.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mic.ctjpmb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nvf.xziqi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://phx.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ztb.gotoacloud.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ssg.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://foc.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://npu.iojbl.cn

[N05] 最大公约数
来源：http://bmt.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://haa.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ctx.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ult.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://els.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cpf.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xru.tanke756.top

Ruby: a.gcd(b)
来源：http://auj.zycfv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oup.guannengcc.top

[N06] 判断回文字符串
来源：http://sik.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://nmv.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://vng.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://bex.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://tvf.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zqi.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://sxh.zhijiandao.cn

Ruby: s == s.reverse
来源：http://wwx.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dma.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://izg.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qzh.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rgw.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hmg.gotoacloud.top

TS:   // 手写 Map<string, number>
来源：http://htl.vqdsnc.cn

Java: // 手写 HashMap
来源：http://pkt.bjfxy.top


<!-- 参考信息 -->