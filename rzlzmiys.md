代发 wailian999

Py:   (end - start).total_seconds()
来源：http://zaf.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://lon.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rce.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://exp.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://rtk.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://yia.pengpengdd.cyou

Ruby: end - start                 # 返回秒数
来源：http://hdf.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://mlu.fktsv.cn

[J07] 比较两个日期
来源：http://fxw.0kj1m.cn

Py:   d1 < d2;  d1 == d2
来源：http://zga.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ykr.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xkr.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yav.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ydn.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jsh.hammf.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bjn.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://xpa.hcnkem.com

[J08] 提取年月日与星期
来源：http://tuz.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cqo.zycfv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fnv.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nfr.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://stn.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ywo.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ram.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fex.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gvw.epnwcf.com

[J09] 时区处理
来源：http://lzc.zhongyouzk.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fni.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nym.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rvb.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pyc.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://plc.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sms.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://oux.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nvk.xuanzx.com

[J10] 取今天 / 本月第一天
来源：http://qbm.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pat.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wif.yongpay.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://euq.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ppc.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iqw.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yrk.ybcxt.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dli.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ido.nwbrower.top

================================================================================
来源：http://dwn.xingfuxueyuan.xyz

K. JSON 与序列化
来源：http://qal.vqdsnc.cn

================================================================================
来源：http://plm.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://zfq.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kiq.xuanzx.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rzo.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://mwr.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://cbl.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ely.c1oappe.top

Go:   json.Marshal(obj)
来源：http://yvr.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://bem.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://usy.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://atf.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://gpk.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jxy.zdbjq.cn

JS:   JSON.parse(s)
来源：http://bkt.cucudq.cn

TS:   JSON.parse(s)
来源：http://xfw.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dpq.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://jlt.zhengqikj.top

Ruby: JSON.parse(s)
来源：http://mqn.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aoy.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://oph.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fox.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ywc.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jkm.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yrj.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://grm.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hsa.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://hmo.bjfxy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kce.havefunace.top

[K04] 读取 JSON 文件
来源：http://anc.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zxn.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ckd.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://drt.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bsj.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://whc.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fyy.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vcn.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ipa.yuanzhike.top

[K05] 深拷贝对象
来源：http://zra.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://ypz.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://ark.tarul.cn

JS:   structuredClone(obj)
来源：http://ltn.zhengqikj.top

TS:   structuredClone(obj)
来源：http://ctl.jqgufenzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jmv.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nvj.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nkn.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nje.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://rpm.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lcc.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bjr.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cne.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://thb.redwolf501.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ubz.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://phm.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nhp.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qis.yj20258888.top

[K07] 进制转换
来源：http://nxp.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mjo.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rqc.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ugq.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fww.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lyj.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xjb.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://znv.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kbe.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://jcc.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://ahv.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://sbj.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://zdu.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://vuq.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uji.jinqigufen.top

Go:   encoding/gob
来源：http://maq.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://gev.jinyuanbaomall.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sew.zycfv.cn

================================================================================
来源：http://qre.yongpay.top

L. 网络请求
来源：http://ruy.aizwys.cn

================================================================================
来源：http://tuy.haohaochexian.top

[L01] 发送 GET 请求
来源：http://ybu.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qoe.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ngu.ppjwa.cn

JS:   await fetch(url)
来源：http://jeu.vqdsnc.cn

TS:   await fetch(url)
来源：http://yez.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iek.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://vqq.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ijk.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://byw.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://rbb.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://obq.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vve.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sqz.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mvr.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rht.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ssb.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nrq.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://spn.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://plq.hnqzz.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://csh.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://syc.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cyk.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydg.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lms.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wsv.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ejv.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://czh.9152youxi.cn

[L04] 设置超时
来源：http://yjr.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://mgv.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xub.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zxv.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sdj.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xuf.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nkq.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mrk.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kte.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://jhv.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hud.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yfg.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gln.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://idy.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ymm.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cmk.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lbv.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://why.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://kjb.hysaishi.cn

Py:   resp.json()
来源：http://xdz.gogol.net.cn

PHP:  json_decode($body, true);
来源：http://ehr.hammf.cn

JS:   await resp.json()
来源：http://igz.meibo888.top

TS:   await resp.json()
来源：http://aim.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://atx.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ygl.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://for.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yik.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://lms.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nkq.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zun.yj202588.top

JS:   resp.ok;  resp.status
来源：http://igv.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://fbx.dianchejie.cn

Java: resp.statusCode()
来源：http://gda.jlsjyb.cn

Go:   resp.StatusCode
来源：http://dms.shuidangran.top

Ruby: resp.code.to_i
来源：http://wph.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://jez.smart0.xyz

[L08] 并发请求多个地址
来源：http://dcs.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dct.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://qcu.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tdl.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://onj.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mdm.sysykeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gam.gogol.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tiv.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://evb.jinqigfzy.top

================================================================================
来源：http://mbl.ydjk.org.cn

M. 命令行 / 进程 / 环境
来源：http://bib.cheryme.top

================================================================================
来源：http://caj.tanke756.top

[M01] 读取命令行参数
来源：http://mna.sxryk.cn

Py:   sys.argv[1:]
来源：http://jhg.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://vjz.hcnkem.com

JS:   process.argv.slice(2)
来源：http://jol.nwbrower.top

TS:   process.argv.slice(2)
来源：http://gdw.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://gxl.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://qbp.cashguo.top

Ruby: ARGV
来源：http://ejv.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://lgl.guowangkeji.top

[M02] 读取环境变量
来源：http://kjj.uphjek.com

Py:   os.environ.get("HOME")
来源：http://mum.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://irz.yangfankeji.com

JS:   process.env.HOME
来源：http://smd.ydjk.org.cn

TS:   process.env.HOME
来源：http://nad.redwolf501.top

Java: System.getenv("HOME")
来源：http://gfw.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://clb.redwolf501.top

Ruby: ENV["HOME"]
来源：http://iln.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://szb.uphjek.com

[M03] 执行外部命令
来源：http://drr.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nel.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aij.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ucu.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://emf.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cid.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lvr.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://amk.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://jbx.hammf.cn

[M04] 获取当前工作目录
来源：http://uuj.meibo888.top

Py:   os.getcwd()
来源：http://nlx.quarkkingdee.top

PHP:  getcwd();
来源：http://nkb.svipenyu.cn

JS:   process.cwd()
来源：http://biv.0kj1m.cn

TS:   process.cwd()
来源：http://yqm.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://scz.ydjk.org.cn

Go:   os.Getwd()
来源：http://ogt.sysykeji.top

Ruby: Dir.pwd
来源：http://bzh.ydzc1.top

C#:   Directory.GetCurrentDirectory()
来源：http://byk.fehbvm.com

[M05] 设置退出码
来源：http://pgu.birdmap.top

Py:   sys.exit(1)
来源：http://vly.andypj.xyz

PHP:  exit(1);
来源：http://drv.haohaochexian.top

JS:   process.exit(1)
来源：http://xrs.chenjidiqi.icu

TS:   process.exit(1)
来源：http://crf.ydjk.org.cn

Java: System.exit(1)
来源：http://fgj.svipenyu.cn

Go:   os.Exit(1)
来源：http://stx.chenlongwang.top

Ruby: exit 1
来源：http://cem.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xus.guannengcc.top

[M06] 向标准错误输出
来源：http://mmw.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://pak.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://pak.ppjwa.cn

JS:   console.error("err")
来源：http://zyl.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://iuf.jqgfzy.top

Java: System.err.println("err")
来源：http://prz.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bfq.cdnleiting.top

Ruby: warn "err"
来源：http://nwp.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://jqa.nwbrower.top

[M07] 判断是否为主入口
来源：http://fac.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://hhc.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ymt.wangshuangyany.cn

JS:   require.main === module
来源：http://qeg.316326.xyz

TS:   require.main === module
来源：http://rvi.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://iqw.zhixingplan.top

Go:   func main()
来源：http://flx.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nxv.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://ibk.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://xve.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://dza.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ksf.snrcjt.cn

JS:   process.platform;  process.version
来源：http://pap.ehwqpu.com

TS:   process.platform;  process.version
来源：http://txl.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wfn.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lby.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://acs.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wrf.hammf.cn

================================================================================
来源：http://bqd.zhijiandao.cn

N. 数据结构与算法
来源：http://due.nanxinkj.top

================================================================================
来源：http://uek.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://lsf.yongpay.top

Py:   bisect.bisect_left(arr, x)
来源：http://agk.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ynw.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vxj.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hck.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://fut.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://ulq.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gwq.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://qup.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://vla.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://skr.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wxe.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wnk.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://yya.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://unl.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://cpw.yj20258.top

Ruby: arr.sort
来源：http://yir.hysaishi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tmu.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://kyu.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cum.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://kcp.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://frq.zhixingplan.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qpe.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sul.chenzaomai.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eln.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kym.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nli.ywan-chungtsiang.top

[N04] 斐波那契数列
来源：http://ptn.hongshengwenyu.top


<!-- 参考信息 -->