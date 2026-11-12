代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jgo.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tfb.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mxg.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://twb.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gfl.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lvh.sxryk.cn

[J09] 时区处理
来源：http://ljy.epnwcf.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tok.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gis.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxe.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://djb.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vef.shanyushiyangtech.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dsa.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://yuj.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sfr.daxiang520.top

[J10] 取今天 / 本月第一天
来源：http://wbk.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sua.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eor.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://idr.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://udu.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://okf.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hpx.c1oappe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ylb.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wkm.yj20258.top

================================================================================
来源：http://phl.hnxiangtu.top

K. JSON 与序列化
来源：http://vum.sxryk.cn

================================================================================
来源：http://pfv.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://tzx.ywan-chungtsiang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bwx.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kdl.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://ntm.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://hjb.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pgb.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://adj.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iqm.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wpg.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://fys.tarul.cn

Py:   json.loads(s)
来源：http://bqb.hysaishi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ybf.yfazqb.com

JS:   JSON.parse(s)
来源：http://vof.bjfxy.top

TS:   JSON.parse(s)
来源：http://ofs.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kaz.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://myj.sysykeji.top

Ruby: JSON.parse(s)
来源：http://pnp.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ddw.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://glk.shanyushiyangtech.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rfw.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ljc.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fbr.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cho.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pti.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bhl.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://qxy.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tpu.pycfn.com

[K04] 读取 JSON 文件
来源：http://zsn.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dvv.hywenlv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rnt.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wjn.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zlr.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qgm.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://opg.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pdt.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bqp.epnwcf.com

[K05] 深拷贝对象
来源：http://cyr.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://xpb.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://bwb.shuidangran.top

JS:   structuredClone(obj)
来源：http://eee.hcnkem.com

TS:   structuredClone(obj)
来源：http://aty.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://fei.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sdt.wangshuangyany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xqb.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rwx.ybcxt.top

[K06] 解析 URL 查询串
来源：http://xxu.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://apk.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://toa.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kjy.jianghu66.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yel.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aic.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zha.andypj.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vsi.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wzc.mhx1999.top

[K07] 进制转换
来源：http://yhw.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nyo.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jhv.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jkk.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://llt.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lam.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xef.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ddd.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yrg.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://zta.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://toc.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://qll.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://yco.bbcook.cn

TS:   v8.serialize(obj)        // Node
来源：http://lqq.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mbf.iojbl.cn

Go:   encoding/gob
来源：http://qmm.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://khm.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oog.jqgufenzy.top

================================================================================
来源：http://fnl.hcnkem.com

L. 网络请求
来源：http://bqv.hfpthk.cn

================================================================================
来源：http://yxt.havefunace.top

[L01] 发送 GET 请求
来源：http://sby.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lic.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ewt.zdqjudy.top

JS:   await fetch(url)
来源：http://kik.cashguo.top

TS:   await fetch(url)
来源：http://tro.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gmh.sweek.top

Go:   resp, err := http.Get(url)
来源：http://hgj.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dol.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eef.yfazqb.com

[L02] 发送 POST JSON
来源：http://bib.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://gml.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tcc.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wli.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wej.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hfu.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://luo.gotoacloud.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jjd.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://urb.zhixingplan.top

[L03] 设置自定义请求头
来源：http://rhx.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xqz.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mfa.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tir.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kzh.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mme.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pks.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://txy.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hes.vqdsnc.cn

[L04] 设置超时
来源：http://adu.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://fdz.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jll.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xmp.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rzn.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ikw.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wdr.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hqp.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wbe.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://evq.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bwr.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hdh.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ieb.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ixd.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xxw.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ikw.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cjl.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ngv.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://odo.ehwqpu.com

Py:   resp.json()
来源：http://oxp.fktsv.cn

PHP:  json_decode($body, true);
来源：http://zwv.dianchejie.cn

JS:   await resp.json()
来源：http://fuu.316326.xyz

TS:   await resp.json()
来源：http://syu.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fta.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://waj.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://rre.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mbm.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://inl.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hmr.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dms.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://ccp.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://tig.yfazqb.com

Java: resp.statusCode()
来源：http://fwa.zhixingplan.top

Go:   resp.StatusCode
来源：http://vpe.zdqjudy.top

Ruby: resp.code.to_i
来源：http://pyn.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://bij.nwbrower.top

[L08] 并发请求多个地址
来源：http://uuy.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lym.guowangkeji.top

PHP:  curl_multi_init() 系列
来源：http://xza.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://loi.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yce.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://njc.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zrg.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wyq.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rjt.fktsv.cn

================================================================================
来源：http://xbn.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://ykr.cashguo.top

================================================================================
来源：http://mci.wangdashe.top

[M01] 读取命令行参数
来源：http://zeu.ppjwa.cn

Py:   sys.argv[1:]
来源：http://xdy.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://jjj.yvedp.cn

JS:   process.argv.slice(2)
来源：http://ntw.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://vug.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://rpi.yvedp.cn

Go:   os.Args[1:]
来源：http://dcw.jqgfzy.top

Ruby: ARGV
来源：http://jqg.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://eak.dianchejie.cn

[M02] 读取环境变量
来源：http://tnr.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://oms.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gsl.jiagoushi.top

JS:   process.env.HOME
来源：http://kxd.nwbrower.top

TS:   process.env.HOME
来源：http://loe.mhx1999.top

Java: System.getenv("HOME")
来源：http://nei.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://smh.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://kia.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ogn.yongpay.top

[M03] 执行外部命令
来源：http://svh.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://anu.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mtj.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pxf.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yoz.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hhr.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tpe.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://qza.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://yuw.birdmap.top

[M04] 获取当前工作目录
来源：http://dgd.shangyingyoupin.top

Py:   os.getcwd()
来源：http://asg.wangdashe.top

PHP:  getcwd();
来源：http://wat.fanxiaobao.xyz

JS:   process.cwd()
来源：http://gok.xuetiantiany.cn

TS:   process.cwd()
来源：http://iij.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cmm.yfazqb.com

Go:   os.Getwd()
来源：http://uhq.jlsjyb.cn

Ruby: Dir.pwd
来源：http://otb.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ksd.pengpengdd.cyou

[M05] 设置退出码
来源：http://dsa.yfazqb.com

Py:   sys.exit(1)
来源：http://xdi.hongshengwenyu.top

PHP:  exit(1);
来源：http://ivw.c1oappe.top

JS:   process.exit(1)
来源：http://hqg.ydzc1.top

TS:   process.exit(1)
来源：http://ewd.guannengcc.top

Java: System.exit(1)
来源：http://pjt.jqgfzy.top

Go:   os.Exit(1)
来源：http://oao.zdqjudy.top

Ruby: exit 1
来源：http://chs.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cvd.cheryme.top

[M06] 向标准错误输出
来源：http://chk.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://bul.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cwe.wangdashe.top

JS:   console.error("err")
来源：http://hab.aizwys.cn

TS:   console.error("err")
来源：http://dds.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://xrc.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vmd.wangshuangyany.cn

Ruby: warn "err"
来源：http://hen.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://jkt.tarul.cn

[M07] 判断是否为主入口
来源：http://oco.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://thi.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pqi.zhengqikj.top

JS:   require.main === module
来源：http://pvl.zhoulong.xyz

TS:   require.main === module
来源：http://xeo.jqgfzy.top

Java: public static void main(String[] args)
来源：http://rqc.sxryk.cn

Go:   func main()
来源：http://yob.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fgm.havefunace.top

C#:   static void Main(string[] args)
来源：http://iwq.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://ope.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://enb.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://zje.epnwcf.com

JS:   process.platform;  process.version
来源：http://hcz.mhx1999.top

TS:   process.platform;  process.version
来源：http://nlm.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ryu.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dgq.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oxs.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ygg.fehbvm.com

================================================================================
来源：http://oyr.vqdsnc.cn

N. 数据结构与算法
来源：http://erg.zhiwuduotai.top

================================================================================
来源：http://duh.pycfn.com

[N01] 二分查找（有序数组）
来源：http://trh.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xwm.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hsc.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tul.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cwl.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://wzx.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://tpr.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://vxp.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://toa.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://zww.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://lme.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://htd.yfazqb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ksn.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cxq.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ojg.fktsv.cn

Go:   slices.Sort(arr)
来源：http://nye.guowangkeji.top

Ruby: arr.sort
来源：http://mil.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aid.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://kxb.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://psf.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://klp.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nnp.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vat.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gyx.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://esk.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rqc.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://wad.wangdashe.top

[N04] 斐波那契数列
来源：http://flg.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jaf.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wnk.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wob.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cxv.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mac.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jmc.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://irc.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ygx.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://mox.hammf.cn

Py:   math.gcd(a, b)
来源：http://mhu.aizwys.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cep.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fzn.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hiy.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yfk.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ryg.fktsv.cn

Ruby: a.gcd(b)
来源：http://qez.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qwp.ydzc1.top

[N06] 判断回文字符串
来源：http://klq.ydzc1.top

Py:   s == s[::-1]
来源：http://vjf.yuxming.cn

PHP:  $s === strrev($s);
来源：http://vxm.shanyushiyangkeji.top


<!-- 参考信息 -->