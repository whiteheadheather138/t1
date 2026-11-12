代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fhj.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://tgq.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qxe.uphjek.com

[J06] 计算两时间之差
来源：http://pkh.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://uue.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://uta.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://olv.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ksv.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://xcx.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://ftk.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://nrj.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://qzs.hysaishi.cn

[J07] 比较两个日期
来源：http://ofs.ivvv.top

Py:   d1 < d2;  d1 == d2
来源：http://aox.yanxiufei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://koh.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://mzd.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://jiq.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wpq.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zpc.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://wio.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://jqt.cqqwz.cn

[J08] 提取年月日与星期
来源：http://abe.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eir.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tep.birdmap.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://avo.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zuk.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yuz.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nrd.chenjidiqi.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ghs.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hto.gogol.net.cn

[J09] 时区处理
来源：http://efp.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://req.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rxh.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oso.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qzd.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zyt.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://faf.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qkj.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tnf.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://jtx.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ozh.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://twj.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bsn.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yvc.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gsi.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lsa.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pae.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nbz.kuanghao11.cn

================================================================================
来源：http://nmh.cdnleiting.top

K. JSON 与序列化
来源：http://veb.zhijiandao.cn

================================================================================
来源：http://gmp.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://olu.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dpr.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aoe.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://tgp.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://pjl.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kqn.vehdjk.com

Go:   json.Marshal(obj)
来源：http://amf.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://baf.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://bpe.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://qky.gotoacloud.top

Py:   json.loads(s)
来源：http://rbe.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fpk.zhoulong.xyz

JS:   JSON.parse(s)
来源：http://hgv.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://fqk.ydzc1.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jvz.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://jct.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://agb.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://apk.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://ucx.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://def.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lua.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jia.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://cjh.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hib.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hcx.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://xsk.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ene.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://lli.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ogf.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ruw.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rsf.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wqy.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jmf.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xjv.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eoj.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fii.yuanzhike.top

[K05] 深拷贝对象
来源：http://fhk.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://lkk.hnqzz.top

PHP:  unserialize(serialize($obj));
来源：http://suk.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://pak.hfpthk.cn

TS:   structuredClone(obj)
来源：http://vqw.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hbe.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://otq.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dng.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ohw.zycfv.cn

[K06] 解析 URL 查询串
来源：http://gci.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://slt.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hvj.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://roe.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mey.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ucm.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sym.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hzi.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ngz.ydjk.org.cn

[K07] 进制转换
来源：http://ull.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gcl.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xhm.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tyd.sxryk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kth.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://chp.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kyz.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dsb.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://csf.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://nip.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://mzc.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://npo.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://jpo.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://crj.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ira.chenzaomai.com

Go:   encoding/gob
来源：http://ecd.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://puw.ppjwa.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qfz.yj202588.top

================================================================================
来源：http://rfh.ywan-chungtsiang.top

L. 网络请求
来源：http://bwz.jinqigfzy.top

================================================================================
来源：http://gzt.svipenyu.cn

[L01] 发送 GET 请求
来源：http://noa.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ikf.jianghu66.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hcn.hesvh.cn

JS:   await fetch(url)
来源：http://fya.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://bza.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rxf.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://mea.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://htv.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bje.yuanzhike.top

[L02] 发送 POST JSON
来源：http://pja.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://rjb.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dzi.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gsf.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gyn.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ovm.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://udz.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://due.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hhd.chenlongwang.top

[L03] 设置自定义请求头
来源：http://amj.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://feo.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wna.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qnw.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vtw.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iun.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jxk.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://izn.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zsj.yongpay.top

[L04] 设置超时
来源：http://kyk.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://qtc.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xcv.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://thl.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tjq.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://knj.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hhu.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vhv.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bst.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://jdl.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kjk.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dhl.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cqc.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bxs.bbcook.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bwy.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nqh.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pdn.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ush.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://bjj.zdqjudy.top

Py:   resp.json()
来源：http://akl.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://ywd.dianchejie.cn

JS:   await resp.json()
来源：http://cfl.fktsv.cn

TS:   await resp.json()
来源：http://nte.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ixi.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aal.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://apl.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xyg.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://dym.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sxq.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nxs.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://fpi.birdmap.top

TS:   resp.ok;  resp.status
来源：http://upx.xylfe.cn

Java: resp.statusCode()
来源：http://goy.ppjwa.cn

Go:   resp.StatusCode
来源：http://jlj.fzhhl.top

Ruby: resp.code.to_i
来源：http://kmm.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://xkr.hfpthk.cn

[L08] 并发请求多个地址
来源：http://yqb.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fjd.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://xsc.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://paz.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lfw.dashuyun.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sfy.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yzo.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uzv.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://isx.yj20258.top

================================================================================
来源：http://eyk.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://bjb.gzhubu.top

================================================================================
来源：http://zet.xziqi.cn

[M01] 读取命令行参数
来源：http://itp.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://pov.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://dbv.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://mqv.iojbl.cn

TS:   process.argv.slice(2)
来源：http://wrn.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://uof.hnqzz.top

Go:   os.Args[1:]
来源：http://fur.haohaochexian.top

Ruby: ARGV
来源：http://atj.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://bxs.xinyue.icu

[M02] 读取环境变量
来源：http://qcg.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://gdd.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jav.fehbvm.com

JS:   process.env.HOME
来源：http://dnx.shuidangran.top

TS:   process.env.HOME
来源：http://nam.cashguo.top

Java: System.getenv("HOME")
来源：http://quw.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://utm.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://ruy.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jny.wangshuangyany.cn

[M03] 执行外部命令
来源：http://yui.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dyk.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xwr.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vec.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ldo.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gml.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uzj.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://mus.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://fyb.xuanzx.com

[M04] 获取当前工作目录
来源：http://ijt.jinqigfzy.top

Py:   os.getcwd()
来源：http://lzj.havefunace.top

PHP:  getcwd();
来源：http://jgv.cdnleiting.top

JS:   process.cwd()
来源：http://wfs.jinghuilouyu.cn

TS:   process.cwd()
来源：http://mvc.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://xcn.redwolf501.top

Go:   os.Getwd()
来源：http://ygh.jiagoushi.top

Ruby: Dir.pwd
来源：http://qil.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ear.chenlongwang.top

[M05] 设置退出码
来源：http://nzf.nwbrower.top

Py:   sys.exit(1)
来源：http://dgu.hongshengwenyu.top

PHP:  exit(1);
来源：http://mpe.mhx1999.top

JS:   process.exit(1)
来源：http://ass.hnqzz.top

TS:   process.exit(1)
来源：http://izg.daria6918.cn

Java: System.exit(1)
来源：http://lnj.snrcjt.cn

Go:   os.Exit(1)
来源：http://vke.pycfn.com

Ruby: exit 1
来源：http://ufr.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hgz.jqgfzy.top

[M06] 向标准错误输出
来源：http://tqg.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://cdk.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vee.chenlongwang.top

JS:   console.error("err")
来源：http://vxd.andypj.xyz

TS:   console.error("err")
来源：http://mbw.gzhubu.top

Java: System.err.println("err")
来源：http://mdu.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rhw.uphjek.com

Ruby: warn "err"
来源：http://bvg.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://yov.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://ouc.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://yrf.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qtz.fengsongda.top

JS:   require.main === module
来源：http://plq.chenzaomai.com

TS:   require.main === module
来源：http://hdh.yj202588.top

Java: public static void main(String[] args)
来源：http://iyp.jiagoushi.top

Go:   func main()
来源：http://crw.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fmx.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://ixl.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://igt.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://upa.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://oos.mhx1999.top

JS:   process.platform;  process.version
来源：http://xei.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://pip.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ape.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mhn.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bfu.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fli.316326.xyz

================================================================================
来源：http://xiu.xylfe.cn

N. 数据结构与算法
来源：http://sew.zhixingplan.top

================================================================================
来源：http://vxs.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://ciq.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fzi.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://arb.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cuh.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gem.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://xeb.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://csw.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://aao.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bmf.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://qcz.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ldn.ehwqpu.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bya.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zxy.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://npz.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oux.zhaomingkeji.xyz

Go:   slices.Sort(arr)
来源：http://jsz.ehwqpu.com

Ruby: arr.sort
来源：http://ura.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://lqs.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://twp.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cyw.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://ycu.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://geq.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://szz.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pxr.zhengqikj.top


<!-- 参考信息 -->