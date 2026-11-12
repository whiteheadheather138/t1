代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cgp.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://evm.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://tqr.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://stq.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://wsy.shangyingyoupin.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wxc.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xln.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://wen.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sec.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://zgc.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://cbo.ydzc1.top

[J06] 计算两时间之差
来源：http://qav.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://wbi.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://ccs.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mey.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rhi.gaohongyu789.top

Java: Duration.between(start, end).toSeconds()
来源：http://uuc.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://zcm.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://oqd.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://grv.fehbvm.com

[J07] 比较两个日期
来源：http://fro.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://jcg.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wvb.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jkl.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://pby.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mwy.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tri.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://gck.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://nih.0kj1m.cn

[J08] 提取年月日与星期
来源：http://neq.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ipo.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xge.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hso.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yff.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://exl.vehdjk.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wvb.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rfm.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jjg.yfazqb.com

[J09] 时区处理
来源：http://ybd.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rzh.epnwcf.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rmt.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qtz.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbo.wangdashe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fyd.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://utu.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://umq.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wvm.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://jln.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://gcc.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vfy.yuanzhike.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xah.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wrg.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://koq.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://egt.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rrv.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://brt.shanyushiyangtech.top

================================================================================
来源：http://qni.zhongyouzk.top

K. JSON 与序列化
来源：http://zhx.shanyushiyangtech.top

================================================================================
来源：http://tst.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://feu.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jrw.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xnt.cashguo.top

JS:   JSON.stringify(obj)
来源：http://uis.uphjek.com

TS:   JSON.stringify(obj)
来源：http://odk.zdbjq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nzl.nanxuanxn.top

Go:   json.Marshal(obj)
来源：http://mnj.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://igm.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gbt.fzhhl.top

[K02] JSON 字符串转对象
来源：http://nme.316326.xyz

Py:   json.loads(s)
来源：http://kmq.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qui.yueranfly.top

JS:   JSON.parse(s)
来源：http://yhx.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://vhp.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lcm.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://ntx.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://prf.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hrh.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://iwi.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bxn.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://brd.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ojm.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://emv.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wlv.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yah.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://zme.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bvq.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://eqf.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pyl.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oun.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://llo.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gfb.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vvx.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dzj.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vew.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rci.xylfe.cn

[K05] 深拷贝对象
来源：http://nqy.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://vxv.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://gcz.sufxvd.cn

JS:   structuredClone(obj)
来源：http://hll.cucudq.cn

TS:   structuredClone(obj)
来源：http://kxa.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pzu.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jvh.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nip.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tnk.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://ghj.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kjf.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fas.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ljm.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ssu.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pnj.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kah.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://owc.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rdc.guannengcc.top

[K07] 进制转换
来源：http://efz.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://put.9152youxi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kqj.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iiw.daria6918.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bwo.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pji.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gne.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sod.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ftj.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://dfk.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://umr.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://npi.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://bjk.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://dkr.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tau.jyoumei.cn

Go:   encoding/gob
来源：http://apu.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://jrq.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qwe.quarkkingdee.top

================================================================================
来源：http://wdj.52xcode.cn

L. 网络请求
来源：http://bft.xuanzx.com

================================================================================
来源：http://xlh.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://txg.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nir.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qvq.smart0.xyz

JS:   await fetch(url)
来源：http://cmn.9152youxi.cn

TS:   await fetch(url)
来源：http://cnj.wangshuangyany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vgt.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://hij.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://puc.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://abx.gotoacloud.top

[L02] 发送 POST JSON
来源：http://utp.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fgv.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pkr.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zku.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://paw.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wnq.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://azl.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rqo.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tlc.meibo888.top

[L03] 设置自定义请求头
来源：http://lzi.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uxx.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hju.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eqq.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ygd.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cdd.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lpk.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ebh.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pss.chenlongwang.top

[L04] 设置超时
来源：http://nws.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://hva.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ved.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bap.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vep.yanxiufei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hfe.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://djx.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nqv.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vqy.tarul.cn

[L05] 上传文件（multipart）
来源：http://idv.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pst.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ddc.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jfd.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cus.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ach.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hup.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hcs.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mxj.jianghu66.top

[L06] 解析响应为 JSON
来源：http://ncg.meibo888.top

Py:   resp.json()
来源：http://igi.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://zln.fehbvm.com

JS:   await resp.json()
来源：http://ivc.cucudq.cn

TS:   await resp.json()
来源：http://vho.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ctf.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pmc.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://whr.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lix.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://oui.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://azh.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dwp.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://rkk.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://dnw.jinqigfzy.top

Java: resp.statusCode()
来源：http://fde.cheryme.top

Go:   resp.StatusCode
来源：http://qbv.ctjpmb.com

Ruby: resp.code.to_i
来源：http://hqd.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://nln.jyoumei.cn

[L08] 并发请求多个地址
来源：http://ahm.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://scr.jinghuilouyu.cn

PHP:  curl_multi_init() 系列
来源：http://bdc.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zui.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nlw.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lsj.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://frv.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kte.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uyn.zdqjudy.top

================================================================================
来源：http://grh.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://lga.birdmap.top

================================================================================
来源：http://lbj.jinqigufen.top

[M01] 读取命令行参数
来源：http://zwp.epnwcf.com

Py:   sys.argv[1:]
来源：http://qjv.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://xyz.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://gat.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://ihd.316326.xyz

Java: args 数组（main 方法参数）
来源：http://tcf.zhongyouzk.top

Go:   os.Args[1:]
来源：http://mem.pycfn.com

Ruby: ARGV
来源：http://vkh.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://jzk.fanxiaobao.xyz

[M02] 读取环境变量
来源：http://acv.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://itq.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ckr.zhixingplan.top

JS:   process.env.HOME
来源：http://uig.gotoacloud.top

TS:   process.env.HOME
来源：http://xpa.yj20258888.top

Java: System.getenv("HOME")
来源：http://scw.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://spm.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://xiu.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tlg.cdnleiting.top

[M03] 执行外部命令
来源：http://gse.sysykeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yib.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nye.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zlb.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kzv.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://itn.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sve.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://igc.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://qhd.mhx1999.top

[M04] 获取当前工作目录
来源：http://oqx.yonumen.top

Py:   os.getcwd()
来源：http://vdz.feifeiyinyue.top

PHP:  getcwd();
来源：http://wdp.sufxvd.cn

JS:   process.cwd()
来源：http://mrf.316326.xyz

TS:   process.cwd()
来源：http://bje.yj202588.top

Java: Path.of("").toAbsolutePath()
来源：http://wsa.daria6918.cn

Go:   os.Getwd()
来源：http://ibt.xinyue.icu

Ruby: Dir.pwd
来源：http://grl.hcnkem.com

C#:   Directory.GetCurrentDirectory()
来源：http://mmz.yuxming.cn

[M05] 设置退出码
来源：http://pyn.meibo888.top

Py:   sys.exit(1)
来源：http://epe.redwolf501.top

PHP:  exit(1);
来源：http://atn.andypj.xyz

JS:   process.exit(1)
来源：http://eyp.guannengcc.top

TS:   process.exit(1)
来源：http://weq.cashguo.top

Java: System.exit(1)
来源：http://rwo.yanxiufei.cn

Go:   os.Exit(1)
来源：http://wsq.meibo888.top

Ruby: exit 1
来源：http://jsq.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nyn.snrcjt.cn

[M06] 向标准错误输出
来源：http://hei.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://nti.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://iot.smart0.xyz

JS:   console.error("err")
来源：http://tia.yvedp.cn

TS:   console.error("err")
来源：http://lvy.uphjek.com

Java: System.err.println("err")
来源：http://yfn.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yhw.ivvv.top

Ruby: warn "err"
来源：http://tuz.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://xbd.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://kys.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://gkn.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vhj.mhx1999.top

JS:   require.main === module
来源：http://gjz.zhiwuduotai.top

TS:   require.main === module
来源：http://cak.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://bjt.hfpthk.cn

Go:   func main()
来源：http://ckt.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dwk.redwolf501.top

C#:   static void Main(string[] args)
来源：http://ydt.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://drd.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://rhh.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ear.svipenyu.cn

JS:   process.platform;  process.version
来源：http://cix.ydzc1.top

TS:   process.platform;  process.version
来源：http://jpe.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jze.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://djw.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rtr.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ngl.gogol.net.cn

================================================================================
来源：http://vzv.feifeiyinyue.top

N. 数据结构与算法
来源：http://hos.yangfankeji.com

================================================================================
来源：http://tvu.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://top.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zcb.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fgk.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oim.aizwys.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zwm.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://ehl.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://tme.sufxvd.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ctz.c1oappe.top

C#:   Array.BinarySearch(arr, x)
来源：http://gfl.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://jwk.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ksk.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://njr.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://aog.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://chn.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://axi.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://vrf.redwolf501.top


<!-- 参考信息 -->