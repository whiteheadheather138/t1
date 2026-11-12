代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://rxj.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://qff.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://eed.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://mwq.aizwys.cn

[J07] 比较两个日期
来源：http://ots.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://dcb.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://upl.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rih.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cin.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ola.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ubz.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://whe.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://mva.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://mpt.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://twc.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zoq.yfazqb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ehv.mhx1999.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dtn.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kud.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jly.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fph.feifeiyinyue.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kgw.fzhhl.top

[J09] 时区处理
来源：http://vlm.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://upd.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bxc.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://keb.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cgn.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://shr.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jff.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dbu.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qdh.cashguo.top

[J10] 取今天 / 本月第一天
来源：http://cbe.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zvz.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bpu.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://msg.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gaw.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://crf.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rmw.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vrn.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mtm.yangfankeji.com

================================================================================
来源：http://srs.cdnleiting.top

K. JSON 与序列化
来源：http://uek.fehbvm.com

================================================================================
来源：http://bbb.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://mgf.quarkkingdee.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://whg.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gwv.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://rmo.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://etd.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://liv.zycfv.cn

Go:   json.Marshal(obj)
来源：http://yrc.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jko.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rdv.yongpay.top

[K02] JSON 字符串转对象
来源：http://jst.zhiwuduotai.top

Py:   json.loads(s)
来源：http://qxj.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ras.fktsv.cn

JS:   JSON.parse(s)
来源：http://kld.yongpay.top

TS:   JSON.parse(s)
来源：http://rup.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xwy.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://kte.guannengcc.top

Ruby: JSON.parse(s)
来源：http://mgx.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wer.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://mhv.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jns.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vih.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wfq.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aaa.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xax.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nob.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://pvr.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ibo.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://zwr.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://clf.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cmj.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aex.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mjb.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://daz.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sra.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zbo.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ifs.yj202588.top

[K05] 深拷贝对象
来源：http://lis.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://zlx.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://usy.fzhhl.top

JS:   structuredClone(obj)
来源：http://oje.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://kkw.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mlo.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cqh.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yzc.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tgw.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://xba.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mfr.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hpy.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oej.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jwj.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zqc.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fsp.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hyg.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bja.chenjidiqi.icu

[K07] 进制转换
来源：http://xko.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dcl.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rca.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vgo.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iti.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wpo.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ipp.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cyz.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wyw.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://hyp.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://gxm.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sqy.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://zok.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://pys.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://utj.zhijiandao.cn

Go:   encoding/gob
来源：http://szz.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://dag.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sbn.tarul.cn

================================================================================
来源：http://efj.316326.xyz

L. 网络请求
来源：http://juo.cheryme.top

================================================================================
来源：http://obu.bjfxy.top

[L01] 发送 GET 请求
来源：http://tpl.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sqy.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://icb.kuanghao11.cn

JS:   await fetch(url)
来源：http://pgw.cucudq.cn

TS:   await fetch(url)
来源：http://dvz.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kbd.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://sno.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yyg.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://urr.wangdashe.top

[L02] 发送 POST JSON
来源：http://wbu.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://tzv.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ups.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://efl.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gti.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://btw.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uum.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ngr.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oxq.ctjpmb.com

[L03] 设置自定义请求头
来源：http://jlm.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rec.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ona.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vmb.jiagoushi.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xqh.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xlv.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iif.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ntl.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yae.pycfn.com

[L04] 设置超时
来源：http://sqg.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://hry.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://elv.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jfs.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nav.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lwf.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://igx.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ofp.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fae.nwbrower.top

[L05] 上传文件（multipart）
来源：http://qso.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ibd.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eub.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://euu.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zrt.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zjx.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sun.jinqigfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ify.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iaf.yfazqb.com

[L06] 解析响应为 JSON
来源：http://lxp.shzxlz.cn

Py:   resp.json()
来源：http://yqk.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://ima.jyoumei.cn

JS:   await resp.json()
来源：http://aok.kuanghao11.cn

TS:   await resp.json()
来源：http://zto.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tgp.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://epi.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://jiw.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kbf.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://yvt.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qdu.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xkc.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://efw.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://gpb.jinyuanbaomall.cn

Java: resp.statusCode()
来源：http://nvd.ppjwa.cn

Go:   resp.StatusCode
来源：http://egg.jyoumei.cn

Ruby: resp.code.to_i
来源：http://ytk.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://xiy.c1oappe.top

[L08] 并发请求多个地址
来源：http://xvj.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://whi.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://sro.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zqt.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bjp.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eir.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wce.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hse.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wcy.yongpay.top

================================================================================
来源：http://kjx.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://jki.cucudq.cn

================================================================================
来源：http://xgq.chenzaomai.com

[M01] 读取命令行参数
来源：http://htn.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://ulo.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://akk.yvedp.cn

JS:   process.argv.slice(2)
来源：http://mpr.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://ems.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://baj.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://oqx.fktsv.cn

Ruby: ARGV
来源：http://sbq.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://iya.yj20258.top

[M02] 读取环境变量
来源：http://zkx.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://ghg.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nua.xylfe.cn

JS:   process.env.HOME
来源：http://ruq.yueranfly.top

TS:   process.env.HOME
来源：http://bbx.hysaishi.cn

Java: System.getenv("HOME")
来源：http://gzr.jqgfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tyb.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://tzt.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lxj.svipenyu.cn

[M03] 执行外部命令
来源：http://pqi.xinyue.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pzo.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xpe.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://udw.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kbe.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yhp.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://epj.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://pdh.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://rco.yj20258888.top

[M04] 获取当前工作目录
来源：http://qbu.pengpengdd.cyou

Py:   os.getcwd()
来源：http://rzh.pengpengdd.cyou

PHP:  getcwd();
来源：http://zef.fzhhl.top

JS:   process.cwd()
来源：http://njj.ybcxt.top

TS:   process.cwd()
来源：http://vyo.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://jsw.hnxiangtu.top

Go:   os.Getwd()
来源：http://cyq.ydjk.org.cn

Ruby: Dir.pwd
来源：http://bzu.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://tpt.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://fxt.vehdjk.com

Py:   sys.exit(1)
来源：http://hfh.jianghu66.top

PHP:  exit(1);
来源：http://stm.hesvh.cn

JS:   process.exit(1)
来源：http://hgz.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://tqb.ctjpmb.com

Java: System.exit(1)
来源：http://rmk.tanke756.top

Go:   os.Exit(1)
来源：http://fxr.jinqigufen.top

Ruby: exit 1
来源：http://bsd.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kvq.xziqi.cn

[M06] 向标准错误输出
来源：http://ksx.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://inc.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vbe.aibaodan.cn

JS:   console.error("err")
来源：http://pfg.daria6918.cn

TS:   console.error("err")
来源：http://plm.xuanzx.com

Java: System.err.println("err")
来源：http://pao.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fix.jlsjyb.cn

Ruby: warn "err"
来源：http://cvd.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://tlg.ydzc1.top

[M07] 判断是否为主入口
来源：http://iiz.tarul.cn

Py:   if __name__ == "__main__":
来源：http://oip.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dza.xinyue.icu

JS:   require.main === module
来源：http://ygp.pycfn.com

TS:   require.main === module
来源：http://wqh.cdnleiting.top

Java: public static void main(String[] args)
来源：http://qxw.hywenlv.cn

Go:   func main()
来源：http://xtp.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ymr.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://pov.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://ybm.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://ehz.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://wsp.tanke756.top

JS:   process.platform;  process.version
来源：http://jva.zhengqikj.top

TS:   process.platform;  process.version
来源：http://mzp.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xcm.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jiw.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qte.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://djv.kuanghao11.cn

================================================================================
来源：http://xiq.dashuyun.cn

N. 数据结构与算法
来源：http://tnz.svipenyu.cn

================================================================================
来源：http://zam.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://uze.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://oae.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wbw.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xtt.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fdl.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bsy.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://dca.fzhhl.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bxj.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://mvs.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://ged.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://dnj.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xgb.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://czk.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://igf.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rqo.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://knk.zdqjudy.top

Ruby: arr.sort
来源：http://bnr.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://plf.tarul.cn

[N03] 快速排序（分治示例）
来源：http://ril.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uvj.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://ozg.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://trm.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ecl.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vvn.shangyingyoupin.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://znq.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yge.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cre.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://tdl.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qyb.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eem.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yhj.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yos.hesvh.cn


<!-- 参考信息 -->