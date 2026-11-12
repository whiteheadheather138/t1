代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rep.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://nsv.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://lbw.hysaishi.cn

[J06] 计算两时间之差
来源：http://sfa.zhaomingkeji.xyz

Py:   (end - start).total_seconds()
来源：http://zxp.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://cek.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://glm.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ctv.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://goh.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://wco.yfazqb.com

Ruby: end - start                 # 返回秒数
来源：http://owd.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://lhk.hysaishi.cn

[J07] 比较两个日期
来源：http://vfg.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://pke.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mof.gaohongyu789.top

JS:   d1.getTime() < d2.getTime()
来源：http://dne.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://len.pycfn.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kza.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rfn.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://nvg.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://rtr.cashguo.top

[J08] 提取年月日与星期
来源：http://xyk.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://avi.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://txj.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hwh.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hun.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vuh.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vkp.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rji.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tzp.fengsongda.top

[J09] 时区处理
来源：http://hvn.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fsn.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://exd.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wdb.xylfe.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cxj.wangshuangyany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lne.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kru.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://glt.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qce.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://iza.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kwp.jqgfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zay.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ukl.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ekc.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qwf.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cze.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jcx.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zyt.yanxiufei.cn

================================================================================
来源：http://pnl.chenjidiqi.icu

K. JSON 与序列化
来源：http://gne.chenjidiqi.icu

================================================================================
来源：http://xfq.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://chl.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mxs.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nqp.tarul.cn

JS:   JSON.stringify(obj)
来源：http://jxg.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://dkj.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fvv.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://dqc.hfpthk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ayg.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wsk.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://nlo.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://von.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://srd.sufxvd.cn

JS:   JSON.parse(s)
来源：http://npa.daria6918.cn

TS:   JSON.parse(s)
来源：http://ijd.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zaa.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://kcp.mhx1999.top

Ruby: JSON.parse(s)
来源：http://nft.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hgj.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://yej.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bwm.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hrd.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://otk.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://npf.cdnleiting.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ovy.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jad.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://nqd.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lxb.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://vwm.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://azd.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ohk.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awv.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nxy.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://psq.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xqo.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pwb.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jmw.aibaodan.cn

[K05] 深拷贝对象
来源：http://vyf.sweek.top

Py:   copy.deepcopy(obj)
来源：http://vpn.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://jrd.tianlin.xyz

JS:   structuredClone(obj)
来源：http://wmf.iojbl.cn

TS:   structuredClone(obj)
来源：http://fzs.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://fau.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://msj.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tab.cdnleiting.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rex.sxryk.cn

[K06] 解析 URL 查询串
来源：http://vyu.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kye.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://icy.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pei.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ypr.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ttx.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gha.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zww.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://msy.aizwys.cn

[K07] 进制转换
来源：http://hrv.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ctn.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nse.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fka.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kml.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ykv.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rst.9152youxi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ani.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gcc.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://xnk.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://vyf.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lfi.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://znd.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://eyj.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fav.gaohongyu789.top

Go:   encoding/gob
来源：http://ekv.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://xey.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rce.ywan-chungtsiang.top

================================================================================
来源：http://hbg.52xcode.cn

L. 网络请求
来源：http://epn.yj20258.top

================================================================================
来源：http://icz.52xcode.cn

[L01] 发送 GET 请求
来源：http://nlk.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ebb.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hoz.mhx1999.top

JS:   await fetch(url)
来源：http://bsh.yvedp.cn

TS:   await fetch(url)
来源：http://ndh.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://msl.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://rga.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qon.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tfp.yfazqb.com

[L02] 发送 POST JSON
来源：http://cwn.pengpengdd.cyou

Py:   requests.post(url, json={"a": 1})
来源：http://xum.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bhp.ydzc1.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://thw.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mpu.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qoa.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://clu.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rzg.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xle.c1oappe.top

[L03] 设置自定义请求头
来源：http://fdn.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ynr.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ozx.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lsb.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qns.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bch.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://skw.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://asz.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pqq.52xcode.cn

[L04] 设置超时
来源：http://wed.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://nmt.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nls.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hfe.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zsi.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://drt.fehbvm.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vrm.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://upw.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://upn.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://pkt.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sgi.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pia.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dof.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ohc.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://emx.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nhz.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wsd.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mic.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://bew.hnqzz.top

Py:   resp.json()
来源：http://wma.cucudq.cn

PHP:  json_decode($body, true);
来源：http://uwk.gogol.net.cn

JS:   await resp.json()
来源：http://buo.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://umw.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://exk.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pjf.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://jkm.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bkn.birdmap.top

[L07] 处理 HTTP 状态码
来源：http://uyx.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://boq.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dyw.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://vjf.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://gvo.birdmap.top

Java: resp.statusCode()
来源：http://sqz.yueranfly.top

Go:   resp.StatusCode
来源：http://zvg.ehwqpu.com

Ruby: resp.code.to_i
来源：http://xno.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://zof.tanke756.top

[L08] 并发请求多个地址
来源：http://vxh.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hxa.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://yex.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ltr.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://awg.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sga.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wxy.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rst.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lei.xuanzx.com

================================================================================
来源：http://kcm.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://zcx.epnwcf.com

================================================================================
来源：http://ufo.tarul.cn

[M01] 读取命令行参数
来源：http://kvy.xziqi.cn

Py:   sys.argv[1:]
来源：http://ecx.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://opn.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://jet.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://uoz.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://hge.xziqi.cn

Go:   os.Args[1:]
来源：http://ket.cdnleiting.top

Ruby: ARGV
来源：http://kqj.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://nli.jianghu66.top

[M02] 读取环境变量
来源：http://ddl.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://iep.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hti.yuanzhike.top

JS:   process.env.HOME
来源：http://jhf.ybcxt.top

TS:   process.env.HOME
来源：http://ela.sxryk.cn

Java: System.getenv("HOME")
来源：http://duc.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fny.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://grz.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hcx.sjlbkw.cn

[M03] 执行外部命令
来源：http://ghp.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://llc.xuetiantiany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kcf.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qye.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://nuf.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://seu.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zct.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://gvt.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://ril.nwbrower.top

[M04] 获取当前工作目录
来源：http://kzt.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://ghc.fktsv.cn

PHP:  getcwd();
来源：http://dov.nwbrower.top

JS:   process.cwd()
来源：http://ims.yj202588.top

TS:   process.cwd()
来源：http://hyd.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://bko.hcnkem.com

Go:   os.Getwd()
来源：http://svy.xziqi.cn

Ruby: Dir.pwd
来源：http://rbj.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://wez.hesvh.cn

[M05] 设置退出码
来源：http://ogl.0kj1m.cn

Py:   sys.exit(1)
来源：http://zax.daria6918.cn

PHP:  exit(1);
来源：http://mem.jiagoushi.top

JS:   process.exit(1)
来源：http://ivl.dianchejie.cn

TS:   process.exit(1)
来源：http://ogk.hnxiangtu.top

Java: System.exit(1)
来源：http://gyr.cdnleiting.top

Go:   os.Exit(1)
来源：http://mif.hesvh.cn

Ruby: exit 1
来源：http://jxc.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nia.hcnkem.com

[M06] 向标准错误输出
来源：http://bkb.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://rad.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://vps.pycfn.com

JS:   console.error("err")
来源：http://yrj.jlsjyb.cn

TS:   console.error("err")
来源：http://unq.jqgufenzy.top

Java: System.err.println("err")
来源：http://ayi.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ufq.shanyushiyangtech.top

Ruby: warn "err"
来源：http://sok.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://vgl.redwolf501.top

[M07] 判断是否为主入口
来源：http://kmx.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://khz.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jzf.ctjpmb.com

JS:   require.main === module
来源：http://tbo.andypj.xyz

TS:   require.main === module
来源：http://xhz.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://koz.shanyushiyangtech.top

Go:   func main()
来源：http://gok.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kqk.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://ilp.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://kxr.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://kmq.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://sqt.hysaishi.cn

JS:   process.platform;  process.version
来源：http://pan.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://wqk.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mue.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hxi.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uac.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://qyi.xziqi.cn

================================================================================
来源：http://xnm.shuidangran.top

N. 数据结构与算法
来源：http://bom.hysaishi.cn

================================================================================
来源：http://uoj.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://bpi.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tle.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jkc.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://odx.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dwe.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://npv.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://rye.hammf.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xqt.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pnh.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://zwf.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://lwg.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://znl.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://hax.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lfr.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bmd.yvedp.cn

Go:   slices.Sort(arr)
来源：http://xqw.cqqwz.cn

Ruby: arr.sort
来源：http://znn.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tdn.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://sup.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dpx.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://rbz.316326.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nzr.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oje.feifeiyinyue.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tcq.tian-w.cn


<!-- 参考信息 -->