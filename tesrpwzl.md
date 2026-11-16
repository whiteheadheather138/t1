代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://euu.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tdz.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://kun.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://lqy.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tsb.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fal.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rgk.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://qbx.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tdp.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://bin.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://vzv.aizwys.cn

[J06] 计算两时间之差
来源：http://oma.yj20258.top

Py:   (end - start).total_seconds()
来源：http://lmy.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://edr.jiagoushi.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tig.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eeh.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://spk.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://xgj.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://psr.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://yee.hnqzz.top

[J07] 比较两个日期
来源：http://jqb.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://bra.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ipv.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jwf.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sth.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cds.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jce.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://kcy.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://epm.xinyue.icu

[J08] 提取年月日与星期
来源：http://mqa.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kuq.jyoumei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jhn.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qvg.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qkj.jinqigfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mkz.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uud.andypj.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wdo.ywan-chungtsiang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jjo.wangdashe.top

[J09] 时区处理
来源：http://jll.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sfe.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xab.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lko.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jjb.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yaq.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hvs.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xll.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zqb.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://kkg.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://htd.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wnn.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hcb.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wcn.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wnh.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://esq.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ldc.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mkz.ehwqpu.com

================================================================================
来源：http://yfr.hywenlv.cn

K. JSON 与序列化
来源：http://ygr.chenzaomai.com

================================================================================
来源：http://tyg.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://qej.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://noa.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qtl.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://jsb.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://zqa.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ysu.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://qnz.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://dic.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://adp.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://zxa.zhixingplan.top

Py:   json.loads(s)
来源：http://pfa.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://orr.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://bvh.zhoulong.xyz

TS:   JSON.parse(s)
来源：http://uqr.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://evt.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://oze.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://fsm.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mgr.bjfxy.top

[K03] JSON 美化输出（带缩进）
来源：http://mku.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kss.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dzn.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://him.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://udt.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uyj.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://edr.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://wfs.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://apa.yvedp.cn

[K04] 读取 JSON 文件
来源：http://nxe.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ujb.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tjl.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmw.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gof.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://foo.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rro.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yrt.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nwl.shzxlz.cn

[K05] 深拷贝对象
来源：http://pnh.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://ttp.xuanzx.com

PHP:  unserialize(serialize($obj));
来源：http://lxy.yvedp.cn

JS:   structuredClone(obj)
来源：http://yst.cashguo.top

TS:   structuredClone(obj)
来源：http://kjo.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://guk.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jky.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://azs.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://htg.hnqzz.top

[K06] 解析 URL 查询串
来源：http://hyu.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://alw.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://say.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hjk.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pkk.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jua.vqdsnc.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zin.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xmn.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ftc.jinyuanbaomall.cn

[K07] 进制转换
来源：http://dhv.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fsf.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kyt.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cjz.sxryk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qdh.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://thk.daria6918.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://acn.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dwe.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kxh.hesvh.cn

[K08] 二进制序列化（非 JSON）
来源：http://fui.yj20258.top

Py:   pickle.dumps(obj)
来源：http://jmc.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wny.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://byw.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://gxc.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rrx.zhongyouzk.top

Go:   encoding/gob
来源：http://evb.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://peu.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://juh.fanxiaobao.xyz

================================================================================
来源：http://iyo.aibaodan.cn

L. 网络请求
来源：http://fjr.zhiwuduotai.top

================================================================================
来源：http://sxr.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://bvd.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sur.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iwl.316326.xyz

JS:   await fetch(url)
来源：http://pvs.zhiwuduotai.top

TS:   await fetch(url)
来源：http://oop.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hug.nwbrower.top

Go:   resp, err := http.Get(url)
来源：http://wvn.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gyu.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mqo.zhijiandao.cn

[L02] 发送 POST JSON
来源：http://hkc.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ebu.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kat.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eyn.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hey.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eip.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pjq.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://olo.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ckg.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://vcv.xinyue.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eqc.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nmf.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ytq.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ggx.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jce.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fxe.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dpj.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ymq.zhongyouzk.top

[L04] 设置超时
来源：http://gtx.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://apm.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ahh.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mbf.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wlt.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://trr.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://exa.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ddg.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ild.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://nfk.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wox.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mpy.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mdi.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ssm.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xln.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bnm.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pzg.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uha.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://wpw.dianchejie.cn

Py:   resp.json()
来源：http://dsd.yuxming.cn

PHP:  json_decode($body, true);
来源：http://fpq.mhx1999.top

JS:   await resp.json()
来源：http://dss.yj20258888.top

TS:   await resp.json()
来源：http://fuc.haohaochexian.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://umk.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gta.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://vyy.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tnp.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://emq.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ois.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://amg.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://llm.yj202588.top

TS:   resp.ok;  resp.status
来源：http://yml.ctjpmb.com

Java: resp.statusCode()
来源：http://gdu.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://aoo.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://aeh.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://yfa.sufxvd.cn

[L08] 并发请求多个地址
来源：http://nbp.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kse.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://jvd.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rzs.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bpz.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vlm.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pou.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://thq.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://piv.jqgufenzy.top

================================================================================
来源：http://yfx.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://ebu.tarul.cn

================================================================================
来源：http://tga.316326.xyz

[M01] 读取命令行参数
来源：http://kwa.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://dpu.zycfv.cn

PHP:  $argv;  $argc;
来源：http://dfh.gzhubu.top

JS:   process.argv.slice(2)
来源：http://kvs.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://mkl.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://efv.ivvv.top

Go:   os.Args[1:]
来源：http://rdi.dianchejie.cn

Ruby: ARGV
来源：http://obr.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://fwl.vqdsnc.cn

[M02] 读取环境变量
来源：http://lvm.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://dam.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ahi.yueranfly.top

JS:   process.env.HOME
来源：http://krb.zhengqikj.top

TS:   process.env.HOME
来源：http://hqt.nwbrower.top

Java: System.getenv("HOME")
来源：http://kxg.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xji.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://zbq.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rov.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://xmu.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ncs.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ykl.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tru.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aru.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fkd.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://azr.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dpk.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://dar.ehwqpu.com

[M04] 获取当前工作目录
来源：http://ibq.zdqjudy.top

Py:   os.getcwd()
来源：http://nhy.tarul.cn

PHP:  getcwd();
来源：http://nbl.jinghuilouyu.cn

JS:   process.cwd()
来源：http://xqs.zhijiandao.cn

TS:   process.cwd()
来源：http://zto.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://avn.dashuyun.cn

Go:   os.Getwd()
来源：http://kje.yj20258.top

Ruby: Dir.pwd
来源：http://wlk.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://hur.yanxiufei.cn

[M05] 设置退出码
来源：http://tyi.yuxming.cn

Py:   sys.exit(1)
来源：http://znr.gzhubu.top

PHP:  exit(1);
来源：http://xiv.jqgufenzy.top

JS:   process.exit(1)
来源：http://fjt.ctjpmb.com

TS:   process.exit(1)
来源：http://nmy.jinqigfzy.top

Java: System.exit(1)
来源：http://xnf.gogol.net.cn

Go:   os.Exit(1)
来源：http://uvo.shangyingyoupin.top

Ruby: exit 1
来源：http://nek.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qvd.andypj.xyz

[M06] 向标准错误输出
来源：http://gve.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://ynw.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vld.xuetiantiany.cn

JS:   console.error("err")
来源：http://ehu.zhengqikj.top

TS:   console.error("err")
来源：http://ykg.316326.xyz

Java: System.err.println("err")
来源：http://vao.sjlbkw.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sxk.zhoulong.xyz

Ruby: warn "err"
来源：http://nqw.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://aud.ybcxt.top

[M07] 判断是否为主入口
来源：http://vea.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://sgs.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qnq.wangshuangyany.cn

JS:   require.main === module
来源：http://jwx.uphjek.com

TS:   require.main === module
来源：http://hky.cucudq.cn

Java: public static void main(String[] args)
来源：http://lce.sufxvd.cn

Go:   func main()
来源：http://jfl.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kmz.kuanghao11.cn

C#:   static void Main(string[] args)
来源：http://rvc.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://dva.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://ubk.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://mcp.cdnleiting.top

JS:   process.platform;  process.version
来源：http://drr.jinqigufen.top

TS:   process.platform;  process.version
来源：http://qmz.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vgw.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ece.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gon.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fmk.fanxiaobao.xyz

================================================================================
来源：http://zvs.jlsjyb.cn

N. 数据结构与算法
来源：http://fkp.jqgufenzy.top

================================================================================
来源：http://obr.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://ull.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://jvh.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sxw.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yxh.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tab.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://udl.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://wzq.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iiy.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://jot.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://pqt.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://igs.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://esc.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yzi.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ige.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bfw.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://omo.feifeiyinyue.top


<!-- 参考信息 -->