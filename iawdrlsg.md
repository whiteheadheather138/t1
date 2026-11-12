代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://xxr.jqgufenzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bhu.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dsz.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://fom.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wcv.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://epa.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ivm.jinqigfzy.top

[J06] 计算两时间之差
来源：http://pyu.hnqzz.top

Py:   (end - start).total_seconds()
来源：http://qrf.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://xgd.tanke756.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vkj.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://spd.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://omy.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://izz.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://hhw.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://oxc.bbcook.cn

[J07] 比较两个日期
来源：http://iol.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://oyr.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vyk.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pzp.pycfn.com

TS:   d1.getTime() < d2.getTime()
来源：http://sfn.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tqo.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dvs.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://uen.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://fkb.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://wfp.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eeh.hfpthk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lqz.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wii.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dua.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vkr.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nmx.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bsn.hongshengwenyu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pog.zhijiandao.cn

[J09] 时区处理
来源：http://rrx.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gxx.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aul.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xpn.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://enx.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mkj.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aix.0kj1m.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mqu.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pcd.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://zmo.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://afv.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kzd.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lgf.jinghuilouyu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fnu.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zdc.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aej.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xkj.cucudq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lvj.fzhhl.top

================================================================================
来源：http://arq.pengpengdd.cyou

K. JSON 与序列化
来源：http://umm.hywenlv.cn

================================================================================
来源：http://skf.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://ief.yangfankeji.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vtv.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xpt.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://sck.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://ptv.bjfxy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://azt.hammf.cn

Go:   json.Marshal(obj)
来源：http://ret.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://kfa.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ite.hesvh.cn

[K02] JSON 字符串转对象
来源：http://thf.shangyingyoupin.top

Py:   json.loads(s)
来源：http://hlk.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ufw.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://gey.shuidangran.top

TS:   JSON.parse(s)
来源：http://oot.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vle.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://vyo.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://zcu.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hrx.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://ane.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wfm.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xan.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ycs.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tpz.ydzc1.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vkx.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://itg.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nfj.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ytl.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://xnr.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pyk.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hxl.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yus.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sxm.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uem.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xlb.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jcb.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cip.chenzaomai.com

[K05] 深拷贝对象
来源：http://ytl.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://xsp.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://pme.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://czw.sysykeji.top

TS:   structuredClone(obj)
来源：http://whj.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://bce.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kie.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://imq.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jnl.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://uld.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nic.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ect.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iei.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ibd.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yjp.xuanzx.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://nuj.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oms.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://raf.ywan-chungtsiang.top

[K07] 进制转换
来源：http://zof.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fap.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qsf.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wsm.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://njo.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rjs.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jfx.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vub.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uga.zdqjudy.top

[K08] 二进制序列化（非 JSON）
来源：http://wrc.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://znk.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rvk.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://ksj.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://uts.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aad.ydzc1.top

Go:   encoding/gob
来源：http://rrw.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://fgw.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yhd.cashguo.top

================================================================================
来源：http://bbn.ywan-chungtsiang.top

L. 网络请求
来源：http://nwa.bbcook.cn

================================================================================
来源：http://sku.sufxvd.cn

[L01] 发送 GET 请求
来源：http://jhq.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lrm.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zdf.snrcjt.cn

JS:   await fetch(url)
来源：http://zoq.zhixingplan.top

TS:   await fetch(url)
来源：http://bhu.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xbl.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://tbn.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wpi.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dod.zhixingplan.top

[L02] 发送 POST JSON
来源：http://fge.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://nyp.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tds.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gcq.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qwp.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hon.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cpf.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hjh.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ffn.xziqi.cn

[L03] 设置自定义请求头
来源：http://ysf.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mze.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zek.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dhw.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xsr.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kyt.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fjr.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://quv.dashuyun.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cpr.jinghuilouyu.cn

[L04] 设置超时
来源：http://wgw.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://qfb.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rhi.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kqg.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nak.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hth.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wpa.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hkd.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sos.smart0.xyz

[L05] 上传文件（multipart）
来源：http://xgp.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mft.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ttm.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gfa.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bjm.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tkz.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qne.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sdr.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dur.uphjek.com

[L06] 解析响应为 JSON
来源：http://nsw.sweek.top

Py:   resp.json()
来源：http://mgo.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://yaz.shuidangran.top

JS:   await resp.json()
来源：http://exu.hnxiangtu.top

TS:   await resp.json()
来源：http://kff.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fxt.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ksb.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://zcg.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vhi.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://pbj.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cdl.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lrd.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://gpp.uphjek.com

TS:   resp.ok;  resp.status
来源：http://jbo.zhoulong.xyz

Java: resp.statusCode()
来源：http://hoo.gaohongyu789.top

Go:   resp.StatusCode
来源：http://tkc.hnqzz.top

Ruby: resp.code.to_i
来源：http://brz.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://dwg.fengsongda.top

[L08] 并发请求多个地址
来源：http://uev.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://grd.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://zxd.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kdq.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kwp.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xqq.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://toi.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mxk.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://typ.yfazqb.com

================================================================================
来源：http://zir.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://nsr.jqgfzy.top

================================================================================
来源：http://mto.gogol.net.cn

[M01] 读取命令行参数
来源：http://kdx.yfazqb.com

Py:   sys.argv[1:]
来源：http://kdu.fzhhl.top

PHP:  $argv;  $argc;
来源：http://gfn.yfazqb.com

JS:   process.argv.slice(2)
来源：http://hhu.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://nzf.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://dkk.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://cfz.snrcjt.cn

Ruby: ARGV
来源：http://flu.bbcook.cn

C#:   args 数组（Main 方法参数）
来源：http://qiy.jlsjyb.cn

[M02] 读取环境变量
来源：http://hvg.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://qam.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xmv.yuanzhike.top

JS:   process.env.HOME
来源：http://yka.hesvh.cn

TS:   process.env.HOME
来源：http://mle.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://vwj.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ugc.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://koh.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ary.jyoumei.cn

[M03] 执行外部命令
来源：http://klv.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ytt.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rex.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kum.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://olp.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://heg.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vkx.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ywn.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://rkk.havefunace.top

[M04] 获取当前工作目录
来源：http://bsd.gogol.net.cn

Py:   os.getcwd()
来源：http://ckl.tianlin.xyz

PHP:  getcwd();
来源：http://dwy.vehdjk.com

JS:   process.cwd()
来源：http://owr.hfpthk.cn

TS:   process.cwd()
来源：http://dvs.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://vpm.shuidangran.top

Go:   os.Getwd()
来源：http://thp.guannengcc.top

Ruby: Dir.pwd
来源：http://lsz.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bcl.jinqigfzy.top

[M05] 设置退出码
来源：http://xfx.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://lkm.xylfe.cn

PHP:  exit(1);
来源：http://xbh.xziqi.cn

JS:   process.exit(1)
来源：http://vcp.redwolf501.top

TS:   process.exit(1)
来源：http://bki.bbcook.cn

Java: System.exit(1)
来源：http://pnc.ydjk.org.cn

Go:   os.Exit(1)
来源：http://oqr.feifeiyinyue.top

Ruby: exit 1
来源：http://xwu.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://axc.c1oappe.top

[M06] 向标准错误输出
来源：http://irp.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://nte.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://lkr.yueranfly.top

JS:   console.error("err")
来源：http://ukd.hammf.cn

TS:   console.error("err")
来源：http://iep.yj20258.top

Java: System.err.println("err")
来源：http://ttz.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yok.gotoacloud.top

Ruby: warn "err"
来源：http://qbz.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://pmi.epnwcf.com

[M07] 判断是否为主入口
来源：http://tyv.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://usw.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vlq.bbcook.cn

JS:   require.main === module
来源：http://rav.sxryk.cn

TS:   require.main === module
来源：http://gpz.birdmap.top

Java: public static void main(String[] args)
来源：http://hjs.dianchejie.cn

Go:   func main()
来源：http://keh.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fko.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://uhb.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://mjw.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://oyj.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://bza.guannengcc.top

JS:   process.platform;  process.version
来源：http://cho.shuidangran.top

TS:   process.platform;  process.version
来源：http://rni.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://csz.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://itj.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dfg.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dor.shuidangran.top

================================================================================
来源：http://taa.zhijiandao.cn

N. 数据结构与算法
来源：http://bhh.jqgfzy.top

================================================================================
来源：http://gtr.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://qcq.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fbx.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://idb.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ckf.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eyr.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fod.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://nqq.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dre.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://nff.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://fey.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://cmj.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tpn.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ptv.sxryk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nvm.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dyu.svipenyu.cn

Go:   slices.Sort(arr)
来源：http://not.birdmap.top

Ruby: arr.sort
来源：http://dod.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rib.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://xrh.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wsz.ydzc1.top


<!-- 参考信息 -->