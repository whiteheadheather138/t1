代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://xij.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ezo.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zeb.chenjidiqi.icu

Java: LocalDate.now().plusDays(7)
来源：http://qwj.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ayf.wangdashe.top

Ruby: Time.now + 7 * 86400
来源：http://gmc.zhongyouzk.top

C#:   DateTime.Now.AddDays(7)
来源：http://kfa.tianlin.xyz

[J06] 计算两时间之差
来源：http://cwd.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://szr.sweek.top

PHP:  $end->diff($start)->days;
来源：http://mvo.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rvi.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lds.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://faa.hysaishi.cn

Go:   end.Sub(start).Hours()
来源：http://fdf.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://kfj.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://kac.aizwys.cn

[J07] 比较两个日期
来源：http://mka.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://adl.sjlbkw.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xty.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://gpq.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://ped.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iia.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ikl.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://xyj.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://fbx.mhx1999.top

[J08] 提取年月日与星期
来源：http://pjz.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fab.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pwd.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dkn.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rht.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://glb.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eaw.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jtp.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ydn.zhengqikj.top

[J09] 时区处理
来源：http://nkc.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uow.cashguo.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ngp.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://myr.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://knn.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://unf.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wft.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vto.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kqw.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://mpg.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bdl.jinghuilouyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xzy.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zqz.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ezb.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://acx.yj20258888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dgp.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rgh.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pyf.yvedp.cn

================================================================================
来源：http://ies.hesvh.cn

K. JSON 与序列化
来源：http://hqk.snrcjt.cn

================================================================================
来源：http://hyf.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://icf.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mcj.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ydr.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://drz.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://bvr.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zae.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://vus.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://qhd.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wky.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://bzf.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://dhq.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uyc.birdmap.top

JS:   JSON.parse(s)
来源：http://ima.guannengcc.top

TS:   JSON.parse(s)
来源：http://bgn.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rfv.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://rqd.cucudq.cn

Ruby: JSON.parse(s)
来源：http://blr.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mal.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://mqr.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hdq.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nhv.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://crp.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ttc.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vfa.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xzx.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xcr.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xol.guowangkeji.top

[K04] 读取 JSON 文件
来源：http://blp.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://snp.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jlk.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gii.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://thh.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mem.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iee.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ued.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fsa.ybcxt.top

[K05] 深拷贝对象
来源：http://rmb.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://mzx.andypj.xyz

PHP:  unserialize(serialize($obj));
来源：http://wra.hysaishi.cn

JS:   structuredClone(obj)
来源：http://xeo.pycfn.com

TS:   structuredClone(obj)
来源：http://iae.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://veh.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rua.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://klc.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://uck.xuanzx.com

[K06] 解析 URL 查询串
来源：http://hxr.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bbw.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tgb.feifeiyinyue.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://chw.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ozc.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sph.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://xwu.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vhh.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lel.cdnleiting.top

[K07] 进制转换
来源：http://swq.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pgr.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xsq.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tfr.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jzt.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gtt.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://etp.xylfe.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qbd.bjfxy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lnb.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://blp.uphjek.com

Py:   pickle.dumps(obj)
来源：http://amq.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tnp.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://bmv.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://pig.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bcv.hywenlv.cn

Go:   encoding/gob
来源：http://rfx.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://yra.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cvw.tian-w.cn

================================================================================
来源：http://cui.wangshuangyany.cn

L. 网络请求
来源：http://bjm.tianlin.xyz

================================================================================
来源：http://hmt.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://tre.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lvj.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xwh.iojbl.cn

JS:   await fetch(url)
来源：http://ipg.fzhhl.top

TS:   await fetch(url)
来源：http://ren.shzxlz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hgn.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://axv.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bqb.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kns.tarul.cn

[L02] 发送 POST JSON
来源：http://snx.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://syy.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vst.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eci.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hfy.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://awd.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jot.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ikk.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hnt.mhx1999.top

[L03] 设置自定义请求头
来源：http://ses.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zee.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mex.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pzj.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cjy.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gna.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kdf.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://btv.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ekw.gogol.net.cn

[L04] 设置超时
来源：http://yki.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://rdr.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ymb.yfazqb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qol.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://efg.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tck.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bhe.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dwv.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tji.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://lqk.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://caq.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nth.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gln.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ulu.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://riv.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://isn.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wxh.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://peu.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://xnf.bbcook.cn

Py:   resp.json()
来源：http://gbj.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://diy.yvedp.cn

JS:   await resp.json()
来源：http://kri.fanxiaobao.xyz

TS:   await resp.json()
来源：http://qcb.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cyh.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fjz.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://vrb.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fwr.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://gqc.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qci.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gne.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://ccm.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://agt.sweek.top

Java: resp.statusCode()
来源：http://els.ydzc1.top

Go:   resp.StatusCode
来源：http://zye.yfazqb.com

Ruby: resp.code.to_i
来源：http://twq.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://jku.yj202588.top

[L08] 并发请求多个地址
来源：http://vdg.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qun.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://wob.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vlu.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://erv.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qee.zhoulong.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ocb.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vbd.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yls.yj202588.top

================================================================================
来源：http://lye.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://gbw.zhixingplan.top

================================================================================
来源：http://boq.ydzc1.top

[M01] 读取命令行参数
来源：http://ebk.hesvh.cn

Py:   sys.argv[1:]
来源：http://msn.yfazqb.com

PHP:  $argv;  $argc;
来源：http://xsh.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://xwn.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://gvz.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://hjf.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://sbj.hongshengwenyu.top

Ruby: ARGV
来源：http://vyw.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://row.jinghuilouyu.cn

[M02] 读取环境变量
来源：http://jug.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://zcf.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ols.jinqigfzy.top

JS:   process.env.HOME
来源：http://tlm.fktsv.cn

TS:   process.env.HOME
来源：http://fmc.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://lan.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bmc.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://drd.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://plu.birdmap.top

[M03] 执行外部命令
来源：http://eic.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uns.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zuo.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rms.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yqo.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bue.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oet.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://ekk.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://zsh.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://ogv.yangfankeji.com

Py:   os.getcwd()
来源：http://nly.yuxming.cn

PHP:  getcwd();
来源：http://qwh.dianchejie.cn

JS:   process.cwd()
来源：http://ynx.iojbl.cn

TS:   process.cwd()
来源：http://jrv.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://cls.chenlongwang.top

Go:   os.Getwd()
来源：http://alj.meibo888.top

Ruby: Dir.pwd
来源：http://kwl.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://jmv.vqdsnc.cn

[M05] 设置退出码
来源：http://aup.gotoacloud.top

Py:   sys.exit(1)
来源：http://hqu.52xcode.cn

PHP:  exit(1);
来源：http://fje.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://tre.ctjpmb.com

TS:   process.exit(1)
来源：http://pwz.xinyue.icu

Java: System.exit(1)
来源：http://joh.nanxinkj.top

Go:   os.Exit(1)
来源：http://azc.ivvv.top

Ruby: exit 1
来源：http://zhd.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kke.ybcxt.top

[M06] 向标准错误输出
来源：http://kbc.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://zfu.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://brr.havefunace.top

JS:   console.error("err")
来源：http://zws.ydjk.org.cn

TS:   console.error("err")
来源：http://eco.tanke756.top

Java: System.err.println("err")
来源：http://ddv.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fqh.nanxinkj.top

Ruby: warn "err"
来源：http://nap.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://lll.bjfxy.top

[M07] 判断是否为主入口
来源：http://stb.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://dgc.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://svt.cdnleiting.top

JS:   require.main === module
来源：http://zef.yongpay.top

TS:   require.main === module
来源：http://csx.svipenyu.cn

Java: public static void main(String[] args)
来源：http://uct.yvedp.cn

Go:   func main()
来源：http://lfl.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zdo.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://ftl.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://kpe.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://ozn.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://not.cheryme.top

JS:   process.platform;  process.version
来源：http://xfc.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://tim.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uzy.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://myg.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vlq.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://pys.zhaomingkeji.xyz

================================================================================
来源：http://lyc.shuidangran.top

N. 数据结构与算法
来源：http://xsr.pengpengdd.cyou

================================================================================
来源：http://flo.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://gmg.hongshengwenyu.top

Py:   bisect.bisect_left(arr, x)
来源：http://mzh.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ruh.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://npj.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rja.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qya.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://npx.cashguo.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ykz.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://lsw.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://qxg.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://yys.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rus.52xcode.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mfv.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://mll.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nto.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://lzj.aizwys.cn

Ruby: arr.sort
来源：http://pvk.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sui.tanke756.top

[N03] 快速排序（分治示例）
来源：http://txo.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ted.svipenyu.cn


<!-- 参考信息 -->