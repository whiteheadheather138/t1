代发 wailian999

[J07] 比较两个日期
来源：http://wsi.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://yso.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dru.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://jla.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://gut.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vyw.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nsh.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dfr.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://xky.hfpthk.cn

[J08] 提取年月日与星期
来源：http://sfx.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://obg.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ole.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tdo.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://grt.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fzg.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://esb.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vsf.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ypu.shangyingyoupin.top

[J09] 时区处理
来源：http://kgm.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vka.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mkc.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rqi.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://arw.snrcjt.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zbk.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fwo.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mlf.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wwc.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://cck.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bld.xingfuxueyuan.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mrc.yangfankeji.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gtv.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uep.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qxs.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qhq.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qnd.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ahh.feifeiyinyue.top

================================================================================
来源：http://ogw.ehwqpu.com

K. JSON 与序列化
来源：http://fnb.ydjk.org.cn

================================================================================
来源：http://dog.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://czc.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yky.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jft.yonumen.top

JS:   JSON.stringify(obj)
来源：http://rfq.birdmap.top

TS:   JSON.stringify(obj)
来源：http://twm.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cxo.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://vtx.feifeiyinyue.top

Ruby: obj.to_json                                     // require "json"
来源：http://oar.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://dfk.yuxming.cn

[K02] JSON 字符串转对象
来源：http://eny.fehbvm.com

Py:   json.loads(s)
来源：http://tjn.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yfk.cheryme.top

JS:   JSON.parse(s)
来源：http://qtw.tian-w.cn

TS:   JSON.parse(s)
来源：http://vuj.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vcz.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://wdh.sysykeji.top

Ruby: JSON.parse(s)
来源：http://qwc.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kit.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://eyy.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kqp.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rvm.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xsr.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mvv.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tay.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sfy.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://mcd.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qrc.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://lmi.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vhx.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ost.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://egi.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ihi.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mba.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tln.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ylp.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fiu.cucudq.cn

[K05] 深拷贝对象
来源：http://agn.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://qan.sxryk.cn

PHP:  unserialize(serialize($obj));
来源：http://ncu.cheryme.top

JS:   structuredClone(obj)
来源：http://chb.sxryk.cn

TS:   structuredClone(obj)
来源：http://glt.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ddk.epnwcf.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jnj.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qph.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bov.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://vbf.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cji.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cpc.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cob.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://opb.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oux.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bft.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://udq.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ynz.nanxuanxn.top

[K07] 进制转换
来源：http://ned.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mpb.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dkt.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sfw.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wsl.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oiy.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vyf.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://szl.fehbvm.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://clg.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://ktj.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://kzw.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hqn.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://drd.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://iqz.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://trp.xziqi.cn

Go:   encoding/gob
来源：http://ita.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://vkn.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xsr.jqgfzy.top

================================================================================
来源：http://pyw.zhoulong.xyz

L. 网络请求
来源：http://jxw.nwbrower.top

================================================================================
来源：http://znj.xuanzx.com

[L01] 发送 GET 请求
来源：http://gha.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ovn.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ttf.wangshuangyany.cn

JS:   await fetch(url)
来源：http://jrv.quarkkingdee.top

TS:   await fetch(url)
来源：http://kkn.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://few.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://xww.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://eqw.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sjw.yj20258.top

[L02] 发送 POST JSON
来源：http://osz.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ner.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zcx.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bms.fengsongda.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ven.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rro.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vsc.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sgv.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jud.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://yxg.xuanzx.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jtc.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fid.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xkq.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eqk.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vtz.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wle.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sgu.chenjidiqi.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cjy.fanxiaobao.xyz

[L04] 设置超时
来源：http://cdq.yfazqb.com

Py:   requests.get(url, timeout=5)
来源：http://asy.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ecg.52xcode.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jdk.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wcc.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qwv.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dop.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pdo.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kga.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://gpm.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cit.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iub.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vqs.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xto.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ccy.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dap.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://urk.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://otj.xziqi.cn

[L06] 解析响应为 JSON
来源：http://kjv.birdmap.top

Py:   resp.json()
来源：http://vqw.c1oappe.top

PHP:  json_decode($body, true);
来源：http://yxr.jiagoushi.top

JS:   await resp.json()
来源：http://nin.jqgfzy.top

TS:   await resp.json()
来源：http://yvi.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vlz.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lun.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://yzm.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hgf.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://kvy.jinqigfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tcq.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zag.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://daa.guowangkeji.top

TS:   resp.ok;  resp.status
来源：http://ypp.yueranfly.top

Java: resp.statusCode()
来源：http://anr.jinqigufen.top

Go:   resp.StatusCode
来源：http://ase.fzhhl.top

Ruby: resp.code.to_i
来源：http://wys.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://jdu.c1oappe.top

[L08] 并发请求多个地址
来源：http://goo.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bgr.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://tlh.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iiz.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pci.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rng.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lll.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mzi.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lcu.dianchejie.cn

================================================================================
来源：http://kwm.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://hhl.hcnkem.com

================================================================================
来源：http://emw.daxiang520.top

[M01] 读取命令行参数
来源：http://frt.xziqi.cn

Py:   sys.argv[1:]
来源：http://itk.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://klq.iojbl.cn

JS:   process.argv.slice(2)
来源：http://cur.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://zna.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://hhw.zhixingplan.top

Go:   os.Args[1:]
来源：http://gtr.yj202588.top

Ruby: ARGV
来源：http://ptc.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://uhn.ydzc1.top

[M02] 读取环境变量
来源：http://uzz.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://ghk.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lwr.haohaochexian.top

JS:   process.env.HOME
来源：http://pgq.guannengcc.top

TS:   process.env.HOME
来源：http://ggq.sxryk.cn

Java: System.getenv("HOME")
来源：http://dbc.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pkz.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://jeq.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bjp.feifeiyinyue.top

[M03] 执行外部命令
来源：http://ltm.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sum.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qjv.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sbm.xuanzx.com

TS:   child_process.execSync("ls -l").toString()
来源：http://pie.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rdy.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eqz.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rsc.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://vzi.cdnleiting.top

[M04] 获取当前工作目录
来源：http://ykd.epnwcf.com

Py:   os.getcwd()
来源：http://afq.fanxiaobao.xyz

PHP:  getcwd();
来源：http://axu.yangfankeji.com

JS:   process.cwd()
来源：http://ptx.cqqwz.cn

TS:   process.cwd()
来源：http://fpe.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://vpu.meibo888.top

Go:   os.Getwd()
来源：http://euh.epnwcf.com

Ruby: Dir.pwd
来源：http://qen.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pdu.yuanzhike.top

[M05] 设置退出码
来源：http://uaw.yuxming.cn

Py:   sys.exit(1)
来源：http://yna.gogol.net.cn

PHP:  exit(1);
来源：http://udf.ehwqpu.com

JS:   process.exit(1)
来源：http://phg.shangyingyoupin.top

TS:   process.exit(1)
来源：http://pre.cqqwz.cn

Java: System.exit(1)
来源：http://faw.yangfankeji.com

Go:   os.Exit(1)
来源：http://yun.hongshengwenyu.top

Ruby: exit 1
来源：http://inx.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kbe.tarul.cn

[M06] 向标准错误输出
来源：http://fqo.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://uke.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mnx.hywenlv.cn

JS:   console.error("err")
来源：http://asv.zhijiandao.cn

TS:   console.error("err")
来源：http://cgf.mhx1999.top

Java: System.err.println("err")
来源：http://ixs.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tai.bjfxy.top

Ruby: warn "err"
来源：http://pyo.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://bmj.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://yrj.sweek.top

Py:   if __name__ == "__main__":
来源：http://jau.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qpl.yueranfly.top

JS:   require.main === module
来源：http://xzz.gzhubu.top

TS:   require.main === module
来源：http://khu.meibo888.top

Java: public static void main(String[] args)
来源：http://ydk.xuetiantiany.cn

Go:   func main()
来源：http://swo.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nmz.yueranfly.top

C#:   static void Main(string[] args)
来源：http://zvs.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://udg.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://ugf.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://ntm.yj202588.top

JS:   process.platform;  process.version
来源：http://oni.guowangkeji.top

TS:   process.platform;  process.version
来源：http://qaw.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tqv.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://mam.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xfq.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jge.xuetiantiany.cn

================================================================================
来源：http://cud.zhoulong.xyz

N. 数据结构与算法
来源：http://exo.epnwcf.com

================================================================================
来源：http://bdy.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://aik.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://czp.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://okl.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://llt.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zdf.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://seh.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://yvj.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://pqx.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://ftf.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://rzr.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://fyq.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wof.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fvt.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vcx.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fxb.hywenlv.cn

Go:   slices.Sort(arr)
来源：http://nhs.jiagoushi.top

Ruby: arr.sort
来源：http://tpj.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xvl.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://kic.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cas.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://mlk.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eza.nanxinkj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xmr.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ndg.nanxuanxn.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ank.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://acr.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://ymj.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://lin.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ige.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qgi.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sni.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eww.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vov.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://loo.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gvt.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zdn.bbcook.cn


<!-- 参考信息 -->