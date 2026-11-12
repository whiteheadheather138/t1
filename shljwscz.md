代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://sfv.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mgk.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ojc.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://ipi.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yvy.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://wfv.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://poa.guannengcc.top

[J06] 计算两时间之差
来源：http://lfh.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://qhv.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://zed.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qib.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dez.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://jco.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://exg.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://naa.sweek.top

C#:   (end - start).TotalSeconds
来源：http://tzz.ivvv.top

[J07] 比较两个日期
来源：http://mge.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://hzw.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bhr.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pym.jinyuanbaomall.cn

TS:   d1.getTime() < d2.getTime()
来源：http://syk.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dla.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rxm.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://ale.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://zxr.yvedp.cn

[J08] 提取年月日与星期
来源：http://nnd.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zdh.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rpy.yfazqb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jet.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rmg.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jpe.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://edp.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tib.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nma.zdbjq.cn

[J09] 时区处理
来源：http://jtk.feifeiyinyue.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kgy.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://goi.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xuk.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baz.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wds.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kvc.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ank.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dmi.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://jaa.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bhl.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ilt.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kuz.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hph.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gdk.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://idz.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kwq.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lpt.sweek.top

================================================================================
来源：http://xrk.sysykeji.top

K. JSON 与序列化
来源：http://jhz.yueranfly.top

================================================================================
来源：http://sub.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://exg.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dtv.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tje.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://jif.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://nys.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qhc.ehwqpu.com

Go:   json.Marshal(obj)
来源：http://hni.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://mrc.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://eez.c1oappe.top

[K02] JSON 字符串转对象
来源：http://plg.jqgfzy.top

Py:   json.loads(s)
来源：http://rsg.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dvx.vehdjk.com

JS:   JSON.parse(s)
来源：http://dhu.yueranfly.top

TS:   JSON.parse(s)
来源：http://fmf.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gol.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://gce.epnwcf.com

Ruby: JSON.parse(s)
来源：http://slm.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dje.daria6918.cn

[K03] JSON 美化输出（带缩进）
来源：http://paa.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sod.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yzz.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nwa.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fbe.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qys.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pss.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://wvr.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qcm.hesvh.cn

[K04] 读取 JSON 文件
来源：http://ebr.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ool.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ysy.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mxw.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yqj.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nyn.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hwg.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ugh.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ykr.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://ary.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://fni.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://rah.cashguo.top

JS:   structuredClone(obj)
来源：http://glj.pycfn.com

TS:   structuredClone(obj)
来源：http://osn.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zdu.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jkx.zhixingplan.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kyd.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fiy.ydzc1.top

[K06] 解析 URL 查询串
来源：http://jhj.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hcg.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rfp.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fzu.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://piu.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kqd.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ren.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://htj.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ekp.zhiwuduotai.top

[K07] 进制转换
来源：http://qmr.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xmk.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://epu.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cbo.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://usn.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ram.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ynl.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ife.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://osm.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://vbr.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://msl.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zwn.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://djh.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://yyj.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dnn.xylfe.cn

Go:   encoding/gob
来源：http://cvr.zhaomingkeji.xyz

Ruby: Marshal.dump(obj)
来源：http://wel.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dgl.jinyuanbaomall.cn

================================================================================
来源：http://tfz.vehdjk.com

L. 网络请求
来源：http://kah.hesvh.cn

================================================================================
来源：http://tpc.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://vgy.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://scf.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lah.chenjidiqi.icu

JS:   await fetch(url)
来源：http://tpl.vehdjk.com

TS:   await fetch(url)
来源：http://ozl.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mkj.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://yex.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xpl.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hdw.zycfv.cn

[L02] 发送 POST JSON
来源：http://jqg.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://pee.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uoj.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lfg.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cxm.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qiu.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://owq.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://anz.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://faf.jyoumei.cn

[L03] 设置自定义请求头
来源：http://omk.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ctu.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vtf.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ass.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iyb.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://phw.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wnh.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ige.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ple.quarkkingdee.top

[L04] 设置超时
来源：http://wyu.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://npj.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pld.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wyy.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tii.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lib.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ocb.zycfv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cpa.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cdw.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://nwo.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kmy.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qsy.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://egy.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qxj.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yzq.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kbf.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qnw.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lql.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://ciw.zdqjudy.top

Py:   resp.json()
来源：http://kbp.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://aru.yvedp.cn

JS:   await resp.json()
来源：http://icw.ivvv.top

TS:   await resp.json()
来源：http://squ.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zeb.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bff.zhijiandao.cn

Ruby: JSON.parse(resp.body)
来源：http://dwa.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ncl.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://htn.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://urt.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qlk.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://hzp.cashguo.top

TS:   resp.ok;  resp.status
来源：http://ehv.daxiang520.top

Java: resp.statusCode()
来源：http://cmv.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://ykq.redwolf501.top

Ruby: resp.code.to_i
来源：http://pmf.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://rdt.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://ojo.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mys.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://qft.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://edu.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ccv.wangshuangyany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://urw.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ihi.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mid.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ogr.cdnleiting.top

================================================================================
来源：http://mwk.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://oyw.gogol.net.cn

================================================================================
来源：http://ekk.andypj.xyz

[M01] 读取命令行参数
来源：http://sod.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://igk.tanke756.top

PHP:  $argv;  $argc;
来源：http://gnb.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://hxh.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://pgp.cqqwz.cn

Java: args 数组（main 方法参数）
来源：http://olc.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://lcu.wangshuangyany.cn

Ruby: ARGV
来源：http://ckc.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://zpz.sysykeji.top

[M02] 读取环境变量
来源：http://dvy.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://owy.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oqi.meibo888.top

JS:   process.env.HOME
来源：http://rpm.iojbl.cn

TS:   process.env.HOME
来源：http://kbk.52xcode.cn

Java: System.getenv("HOME")
来源：http://vdu.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yol.xinyue.icu

Ruby: ENV["HOME"]
来源：http://ahe.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hxj.havefunace.top

[M03] 执行外部命令
来源：http://dem.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gqk.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jrm.zdbjq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ixt.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pnj.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vca.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hke.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wzs.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://voa.0kj1m.cn

[M04] 获取当前工作目录
来源：http://ycb.epnwcf.com

Py:   os.getcwd()
来源：http://nrk.zycfv.cn

PHP:  getcwd();
来源：http://zfw.fanxiaobao.xyz

JS:   process.cwd()
来源：http://nia.sysykeji.top

TS:   process.cwd()
来源：http://tib.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://azf.cheryme.top

Go:   os.Getwd()
来源：http://khc.shzxlz.cn

Ruby: Dir.pwd
来源：http://gvj.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tgv.redwolf501.top

[M05] 设置退出码
来源：http://nfv.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://xmo.jlsjyb.cn

PHP:  exit(1);
来源：http://eip.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://ifd.dashuyun.cn

TS:   process.exit(1)
来源：http://ihf.andypj.xyz

Java: System.exit(1)
来源：http://eqo.gzhubu.top

Go:   os.Exit(1)
来源：http://pom.yfazqb.com

Ruby: exit 1
来源：http://igv.chenlongwang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://civ.quarkkingdee.top

[M06] 向标准错误输出
来源：http://nqo.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://cej.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mgf.feifeiyinyue.top

JS:   console.error("err")
来源：http://qjw.zdbjq.cn

TS:   console.error("err")
来源：http://cog.fzhhl.top

Java: System.err.println("err")
来源：http://qke.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sgz.daxiang520.top

Ruby: warn "err"
来源：http://lmj.sweek.top

C#:   Console.Error.WriteLine("err")
来源：http://yeq.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://cll.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://uhy.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://exb.cdnleiting.top

JS:   require.main === module
来源：http://wod.gogol.net.cn

TS:   require.main === module
来源：http://bqc.cashguo.top

Java: public static void main(String[] args)
来源：http://cnw.guowangkeji.top

Go:   func main()
来源：http://ppv.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zrq.pycfn.com

C#:   static void Main(string[] args)
来源：http://psj.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://urb.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://aka.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://cqq.xuanzx.com

JS:   process.platform;  process.version
来源：http://dkj.hesvh.cn

TS:   process.platform;  process.version
来源：http://him.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zuc.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jyu.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wer.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mvu.zhiwuduotai.top

================================================================================
来源：http://lpf.chenjidiqi.icu

N. 数据结构与算法
来源：http://vyi.chenzaomai.com

================================================================================
来源：http://utp.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://esm.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://ocr.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ago.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://naa.jinghuilouyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nsc.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://acf.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://irp.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mmd.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://ied.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://cxj.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://mfc.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wql.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qor.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vys.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fmb.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://fvr.fehbvm.com

Ruby: arr.sort
来源：http://lug.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://cex.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://gay.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cdv.bjfxy.top


<!-- 参考信息 -->