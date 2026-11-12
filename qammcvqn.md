代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://jsf.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ggr.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yck.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://iir.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jbe.nanxuanxn.top

Ruby: Time.now + 7 * 86400
来源：http://gst.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://hsq.zhengqikj.top

[J06] 计算两时间之差
来源：http://dnj.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://qom.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://egr.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fmh.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jzv.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://dgd.shanyushiyangkeji.top

Go:   end.Sub(start).Hours()
来源：http://cfc.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://aur.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://bqb.wangshuangyany.cn

[J07] 比较两个日期
来源：http://rvm.svipenyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://icv.cheryme.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iyh.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ttx.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://usu.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jyu.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://djn.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://ppy.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://chg.daxiang520.top

[J08] 提取年月日与星期
来源：http://dqz.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hqa.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kaa.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dih.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kai.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gqi.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bhl.ybcxt.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wmx.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://idr.hfpthk.cn

[J09] 时区处理
来源：http://amn.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nvk.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hbo.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://scq.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ouf.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hiv.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aog.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xyf.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wrs.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://cso.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://moo.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lbf.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nul.fzhhl.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mdk.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fod.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bgu.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jsv.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ujw.chenjidiqi.icu

================================================================================
来源：http://lbu.sufxvd.cn

K. JSON 与序列化
来源：http://qji.pycfn.com

================================================================================
来源：http://pgm.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://xqk.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bzv.fehbvm.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pda.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://ydt.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://dbf.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cyd.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://otq.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://nib.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ehq.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://wqk.9152youxi.cn

Py:   json.loads(s)
来源：http://efn.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ftg.hfpthk.cn

JS:   JSON.parse(s)
来源：http://ppp.gzhubu.top

TS:   JSON.parse(s)
来源：http://pay.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hbg.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://spr.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://qsz.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fuz.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://aln.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xmh.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://onz.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bll.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://asl.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gns.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ynj.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://gnw.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hos.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://fgl.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pmk.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xjw.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hte.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://crp.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gxc.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qez.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hzs.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zzo.0kj1m.cn

[K05] 深拷贝对象
来源：http://rlo.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://slx.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://clv.cashguo.top

JS:   structuredClone(obj)
来源：http://soa.nwbrower.top

TS:   structuredClone(obj)
来源：http://eqr.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wzu.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vmt.jlsjyb.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tgz.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qbb.52xcode.cn

[K06] 解析 URL 查询串
来源：http://knv.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ler.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://our.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tqc.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tnz.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zjp.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mau.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uln.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eqi.snrcjt.cn

[K07] 进制转换
来源：http://aum.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://etj.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kkq.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://spv.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jup.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jip.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vjb.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rrq.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sqn.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://xcf.yuxming.cn

Py:   pickle.dumps(obj)
来源：http://ubh.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zzx.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://xmo.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://rbt.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dgf.hcnkem.com

Go:   encoding/gob
来源：http://loh.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://yoy.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ytc.jyoumei.cn

================================================================================
来源：http://qju.havefunace.top

L. 网络请求
来源：http://ejp.yj202588.top

================================================================================
来源：http://wya.52xcode.cn

[L01] 发送 GET 请求
来源：http://sbi.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://adj.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gkx.zdbjq.cn

JS:   await fetch(url)
来源：http://jcl.gaohongyu789.top

TS:   await fetch(url)
来源：http://hax.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cnb.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://ghy.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://thr.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kuk.yuanzhike.top

[L02] 发送 POST JSON
来源：http://uuc.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://tcf.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wjb.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ofi.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dww.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mkm.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://obo.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hpb.nanxinkj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wbk.redwolf501.top

[L03] 设置自定义请求头
来源：http://uuc.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xvh.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lwi.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://phe.sysykeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ebx.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://szm.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://apr.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tlr.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gds.daxiang520.top

[L04] 设置超时
来源：http://njn.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://vft.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ixd.daxiang520.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ilq.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xmr.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pdo.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xrt.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://upn.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zkx.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://bfs.daria6918.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ngs.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uvm.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rqz.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kbg.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://txx.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lda.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tqf.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://thw.guannengcc.top

[L06] 解析响应为 JSON
来源：http://ejv.aizwys.cn

Py:   resp.json()
来源：http://cvx.52xcode.cn

PHP:  json_decode($body, true);
来源：http://qhr.zdbjq.cn

JS:   await resp.json()
来源：http://rzl.uphjek.com

TS:   await resp.json()
来源：http://xsy.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jrm.jinyuanbaomall.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qfx.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://pjq.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://acs.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://syx.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hov.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ywm.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://jku.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://xbr.chenlongwang.top

Java: resp.statusCode()
来源：http://wqd.ybcxt.top

Go:   resp.StatusCode
来源：http://akz.ybcxt.top

Ruby: resp.code.to_i
来源：http://kjc.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://cuh.daria6918.cn

[L08] 并发请求多个地址
来源：http://tlj.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tgq.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://pwd.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sti.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mop.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lvk.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://czr.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fuj.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pjf.zhoulong.xyz

================================================================================
来源：http://wvj.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://nvq.hnqzz.top

================================================================================
来源：http://emg.kuanghao11.cn

[M01] 读取命令行参数
来源：http://kid.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://rqh.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://wjp.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://gzc.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://qdm.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://yos.wangdashe.top

Go:   os.Args[1:]
来源：http://hks.hongshengwenyu.top

Ruby: ARGV
来源：http://iew.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://dnf.dianchejie.cn

[M02] 读取环境变量
来源：http://poz.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://aiy.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://upx.aibaodan.cn

JS:   process.env.HOME
来源：http://kls.gogol.net.cn

TS:   process.env.HOME
来源：http://brc.daxiang520.top

Java: System.getenv("HOME")
来源：http://srr.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fye.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://zjv.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ipm.vqdsnc.cn

[M03] 执行外部命令
来源：http://nds.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pys.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://owo.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://csn.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cio.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eaa.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://qoz.chenjidiqi.icu

Ruby: system("ls -l");  `ls -l`
来源：http://mlp.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://nds.sxryk.cn

[M04] 获取当前工作目录
来源：http://vow.sxryk.cn

Py:   os.getcwd()
来源：http://khj.gzhubu.top

PHP:  getcwd();
来源：http://gzx.fktsv.cn

JS:   process.cwd()
来源：http://fwx.jianghu66.top

TS:   process.cwd()
来源：http://nxe.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://jvs.tianlin.xyz

Go:   os.Getwd()
来源：http://uxw.ehwqpu.com

Ruby: Dir.pwd
来源：http://tia.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qwk.0kj1m.cn

[M05] 设置退出码
来源：http://pzk.shanyushiyangtech.top

Py:   sys.exit(1)
来源：http://fsx.yangfankeji.com

PHP:  exit(1);
来源：http://ffy.uphjek.com

JS:   process.exit(1)
来源：http://uye.52xcode.cn

TS:   process.exit(1)
来源：http://pfc.yuxming.cn

Java: System.exit(1)
来源：http://dgh.yj20258888.top

Go:   os.Exit(1)
来源：http://loz.wangdashe.top

Ruby: exit 1
来源：http://gtk.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cmr.wangdashe.top

[M06] 向标准错误输出
来源：http://tqv.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://kdw.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xfz.jqgufenzy.top

JS:   console.error("err")
来源：http://hbd.haohaochexian.top

TS:   console.error("err")
来源：http://cyi.shanyushiyangkeji.top

Java: System.err.println("err")
来源：http://uev.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://chm.zdbjq.cn

Ruby: warn "err"
来源：http://yha.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://dgz.shuidangran.top

[M07] 判断是否为主入口
来源：http://xwf.pycfn.com

Py:   if __name__ == "__main__":
来源：http://aio.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://efh.yongpay.top

JS:   require.main === module
来源：http://win.chenzaomai.com

TS:   require.main === module
来源：http://vlo.aibaodan.cn

Java: public static void main(String[] args)
来源：http://tni.tianlin.xyz

Go:   func main()
来源：http://whx.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tgl.ydzc1.top

C#:   static void Main(string[] args)
来源：http://zsq.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://dmm.ydzc1.top

Py:   platform.system();  platform.python_version()
来源：http://ukl.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://qab.yongpay.top

JS:   process.platform;  process.version
来源：http://ifj.jyoumei.cn

TS:   process.platform;  process.version
来源：http://umj.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ayo.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qtw.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ogp.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fgo.nwbrower.top

================================================================================
来源：http://gnp.shuidangran.top

N. 数据结构与算法
来源：http://qtu.jianghu66.top

================================================================================
来源：http://sfa.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://fxp.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://qmp.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uqm.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vvc.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bch.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://bju.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://riw.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://cxv.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ngq.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://efh.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://ouj.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fpc.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://glk.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qro.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ukw.yueranfly.top

Go:   slices.Sort(arr)
来源：http://tpd.vqdsnc.cn

Ruby: arr.sort
来源：http://yzj.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mfh.cheryme.top

[N03] 快速排序（分治示例）
来源：http://wcq.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kkb.xylfe.cn


<!-- 参考信息 -->