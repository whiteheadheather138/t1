代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://ykb.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://qxw.guannengcc.top

Ruby: end - start                 # 返回秒数
来源：http://lum.nwbrower.top

C#:   (end - start).TotalSeconds
来源：http://rdy.9152youxi.cn

[J07] 比较两个日期
来源：http://cnx.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://vge.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hqk.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://tow.daria6918.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kxh.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aeh.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vds.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://rmp.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://vhw.jinghuilouyu.cn

[J08] 提取年月日与星期
来源：http://eas.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zou.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vep.shanyushiyangtech.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kym.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hql.gzhubu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://art.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qoe.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://plp.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ygk.quarkkingdee.top

[J09] 时区处理
来源：http://zyc.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dhq.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://biq.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://abr.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rce.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://poa.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zsh.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oid.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qlj.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://qof.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jzu.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yyl.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kxu.gogol.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kja.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wmr.epnwcf.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xis.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bue.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://exi.jinqigfzy.top

================================================================================
来源：http://ydm.xziqi.cn

K. JSON 与序列化
来源：http://vba.cheryme.top

================================================================================
来源：http://jlw.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://elr.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qgu.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qsk.ehwqpu.com

JS:   JSON.stringify(obj)
来源：http://lpo.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://ndr.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vto.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://tft.ydjk.org.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sxq.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ftr.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://ncr.ehwqpu.com

Py:   json.loads(s)
来源：http://nzz.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yhc.gzhubu.top

JS:   JSON.parse(s)
来源：http://avg.tanke756.top

TS:   JSON.parse(s)
来源：http://chx.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hri.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://xqq.nwbrower.top

Ruby: JSON.parse(s)
来源：http://mgv.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mce.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://sfw.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://huo.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://krd.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://aqy.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mut.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tif.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ele.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://owx.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lxa.yj20258888.top

[K04] 读取 JSON 文件
来源：http://yjh.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qzy.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lyg.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zel.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xyl.gaohongyu789.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://any.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wmy.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hlf.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qtp.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://iyn.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://frj.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://cns.daxiang520.top

JS:   structuredClone(obj)
来源：http://rzx.andypj.xyz

TS:   structuredClone(obj)
来源：http://wzc.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://irq.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jlc.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://icy.fengsongda.top

C#:   // 序列化往返，或自定义 Clone
来源：http://whq.tian-w.cn

[K06] 解析 URL 查询串
来源：http://ohn.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wgo.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://efc.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bsp.jianghu66.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qdb.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wby.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cwv.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://upk.zhengqikj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fmb.c1oappe.top

[K07] 进制转换
来源：http://bvu.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nft.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vqm.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sdd.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jtv.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yye.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cvk.svipenyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://afp.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hel.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://oph.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://yyj.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ivp.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://who.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://mne.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iwj.shanyushiyangkeji.top

Go:   encoding/gob
来源：http://vub.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://qwk.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hxn.sysykeji.top

================================================================================
来源：http://fgt.xuanzx.com

L. 网络请求
来源：http://xel.wangdashe.top

================================================================================
来源：http://mab.jinqigufen.top

[L01] 发送 GET 请求
来源：http://ozz.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ulq.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oir.shuidangran.top

JS:   await fetch(url)
来源：http://fii.jqgfzy.top

TS:   await fetch(url)
来源：http://zbt.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ybi.shuidangran.top

Go:   resp, err := http.Get(url)
来源：http://tpr.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://avb.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kjk.yvedp.cn

[L02] 发送 POST JSON
来源：http://uvz.vehdjk.com

Py:   requests.post(url, json={"a": 1})
来源：http://aiv.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://frs.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kmp.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wkw.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://awu.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wlc.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xlb.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ebw.chenzaomai.com

[L03] 设置自定义请求头
来源：http://oka.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wsl.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vtx.zhiwuduotai.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://chu.sjlbkw.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nkv.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jcd.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ppn.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://asb.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ysg.shangyingyoupin.top

[L04] 设置超时
来源：http://cnu.yangfankeji.com

Py:   requests.get(url, timeout=5)
来源：http://teh.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ryr.jqgfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tjf.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eda.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dwa.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nlm.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vcb.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nmi.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://uqf.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sqf.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://twq.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bgt.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vsd.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hfk.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dvh.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://usk.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yaw.ydzc1.top

[L06] 解析响应为 JSON
来源：http://dst.haohaochexian.top

Py:   resp.json()
来源：http://kgw.ybcxt.top

PHP:  json_decode($body, true);
来源：http://avm.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://cjc.jianghu66.top

TS:   await resp.json()
来源：http://bfo.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://umi.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ehz.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://dcb.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hah.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://guh.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gcw.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://byg.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://zxr.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://nqk.hesvh.cn

Java: resp.statusCode()
来源：http://olg.hammf.cn

Go:   resp.StatusCode
来源：http://pyh.guannengcc.top

Ruby: resp.code.to_i
来源：http://gkj.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://yjc.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://vmp.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hge.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://kqg.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ofw.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://suz.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dnq.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gin.hongshengwenyu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://osp.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sej.sweek.top

================================================================================
来源：http://kks.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://sxy.xinyue.icu

================================================================================
来源：http://ydd.epnwcf.com

[M01] 读取命令行参数
来源：http://uhk.tian-w.cn

Py:   sys.argv[1:]
来源：http://giw.redwolf501.top

PHP:  $argv;  $argc;
来源：http://rsr.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://zuj.vehdjk.com

TS:   process.argv.slice(2)
来源：http://mij.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://bbp.yj20258.top

Go:   os.Args[1:]
来源：http://nwg.tian-w.cn

Ruby: ARGV
来源：http://ivf.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://sdx.aibaodan.cn

[M02] 读取环境变量
来源：http://zeq.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://fse.smart0.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bvq.zdbjq.cn

JS:   process.env.HOME
来源：http://yhq.hfpthk.cn

TS:   process.env.HOME
来源：http://btt.daxiang520.top

Java: System.getenv("HOME")
来源：http://tcf.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://adl.andypj.xyz

Ruby: ENV["HOME"]
来源：http://jbu.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qvf.ydjk.org.cn

[M03] 执行外部命令
来源：http://kpw.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wyi.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gom.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dqc.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://drb.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ezx.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://blb.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://pcl.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://keb.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://zew.quarkkingdee.top

Py:   os.getcwd()
来源：http://fqf.iojbl.cn

PHP:  getcwd();
来源：http://gbn.cheryme.top

JS:   process.cwd()
来源：http://kzs.dianchejie.cn

TS:   process.cwd()
来源：http://otv.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://oxb.hywenlv.cn

Go:   os.Getwd()
来源：http://ytk.tanke756.top

Ruby: Dir.pwd
来源：http://unx.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wsp.chenlongwang.top

[M05] 设置退出码
来源：http://vfj.bbcook.cn

Py:   sys.exit(1)
来源：http://lxi.gotoacloud.top

PHP:  exit(1);
来源：http://dev.yangfankeji.com

JS:   process.exit(1)
来源：http://ccz.hammf.cn

TS:   process.exit(1)
来源：http://lwk.yueranfly.top

Java: System.exit(1)
来源：http://nzt.meibo888.top

Go:   os.Exit(1)
来源：http://hrl.yfazqb.com

Ruby: exit 1
来源：http://vix.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://idw.cashguo.top

[M06] 向标准错误输出
来源：http://fpj.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://vlq.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oca.yvedp.cn

JS:   console.error("err")
来源：http://mwc.tianlin.xyz

TS:   console.error("err")
来源：http://vmq.gzhubu.top

Java: System.err.println("err")
来源：http://kxi.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://crt.quarkkingdee.top

Ruby: warn "err"
来源：http://pnw.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://ndj.yongpay.top

[M07] 判断是否为主入口
来源：http://nmp.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://lar.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hub.fengsongda.top

JS:   require.main === module
来源：http://wlm.jinyuanbaomall.cn

TS:   require.main === module
来源：http://wic.redwolf501.top

Java: public static void main(String[] args)
来源：http://iyg.jinqigfzy.top

Go:   func main()
来源：http://ldj.jinqigfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ydh.hnqzz.top

C#:   static void Main(string[] args)
来源：http://ekx.yj20258.top

[M08] 获取系统与运行时信息
来源：http://ysx.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://lof.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://pth.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://ybe.zdbjq.cn

TS:   process.platform;  process.version
来源：http://wfv.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pfb.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yix.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lnr.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zfn.yuanzhike.top

================================================================================
来源：http://fhw.xuanzx.com

N. 数据结构与算法
来源：http://qco.xuetiantiany.cn

================================================================================
来源：http://qgo.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://ioy.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://khe.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qae.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kik.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hsy.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hst.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://muw.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://nuj.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xoa.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://rft.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://rlt.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vtn.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pfd.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zsg.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jep.epnwcf.com

Go:   slices.Sort(arr)
来源：http://duf.wangdashe.top

Ruby: arr.sort
来源：http://vsq.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://plo.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://uon.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vdb.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://vwn.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fdw.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iba.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://amw.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rom.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zde.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://qkk.kuanghao11.cn

[N04] 斐波那契数列
来源：http://hjc.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xyu.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kws.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hqb.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xry.zhiwuduotai.top


<!-- 参考信息 -->