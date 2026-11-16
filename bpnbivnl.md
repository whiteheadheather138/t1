代发 wailian999

[J07] 比较两个日期
来源：http://gkj.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://tob.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lug.shanyushiyangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://xmx.haohaochexian.top

TS:   d1.getTime() < d2.getTime()
来源：http://yva.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://foa.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://esq.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xxc.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://vzh.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://lmb.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lyj.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qzo.zhaomingkeji.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hty.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vgj.redwolf501.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fad.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nfa.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vuq.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dmi.jiagoushi.top

[J09] 时区处理
来源：http://iym.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bod.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lnk.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fun.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://asv.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://isc.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yza.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vkb.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lox.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://qbj.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://yeo.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wzk.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://udo.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ruj.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fwm.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lyu.yongpay.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eir.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lto.ywan-chungtsiang.top

================================================================================
来源：http://okm.hysaishi.cn

K. JSON 与序列化
来源：http://niv.hywenlv.cn

================================================================================
来源：http://hrc.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://qxk.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yzl.hysaishi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eaq.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://kfb.xingfuxueyuan.xyz

TS:   JSON.stringify(obj)
来源：http://mxl.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://afr.bjfxy.top

Go:   json.Marshal(obj)
来源：http://xbn.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://fzr.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aqr.epnwcf.com

[K02] JSON 字符串转对象
来源：http://qta.xylfe.cn

Py:   json.loads(s)
来源：http://fez.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jac.ybcxt.top

JS:   JSON.parse(s)
来源：http://feg.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://rwy.hywenlv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://olb.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://bwj.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://pnh.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gcp.tanke756.top

[K03] JSON 美化输出（带缩进）
来源：http://vqo.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jts.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tzy.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://thd.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://iyx.jinqigfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lrg.ydjk.org.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jsv.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nju.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://shm.epnwcf.com

[K04] 读取 JSON 文件
来源：http://rwu.xuanzx.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ybz.ehwqpu.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iat.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bzz.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ehy.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yph.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kfw.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://she.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kad.fengsongda.top

[K05] 深拷贝对象
来源：http://dgh.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://veb.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://nim.hammf.cn

JS:   structuredClone(obj)
来源：http://vrq.zhengqikj.top

TS:   structuredClone(obj)
来源：http://kok.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://and.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gks.yuanzhike.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kwv.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pla.haohaochexian.top

[K06] 解析 URL 查询串
来源：http://kos.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uvj.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nyp.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jwq.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://svr.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wif.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fwg.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fcn.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hsj.quarkkingdee.top

[K07] 进制转换
来源：http://muy.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ane.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wis.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mni.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://idy.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://unb.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cen.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xdj.xuetiantiany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oqz.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://jgu.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://tkz.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gok.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://qoj.daxiang520.top

TS:   v8.serialize(obj)        // Node
来源：http://qcw.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lgp.zhengqikj.top

Go:   encoding/gob
来源：http://swm.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://jxw.daria6918.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nww.yangfankeji.com

================================================================================
来源：http://ezt.vqdsnc.cn

L. 网络请求
来源：http://lel.chenjidiqi.icu

================================================================================
来源：http://idv.0kj1m.cn

[L01] 发送 GET 请求
来源：http://irn.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vmr.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://plj.jlsjyb.cn

JS:   await fetch(url)
来源：http://gys.hnqzz.top

TS:   await fetch(url)
来源：http://gdd.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vnk.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://bbr.vqdsnc.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hca.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gzx.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://rbo.yuxming.cn

Py:   requests.post(url, json={"a": 1})
来源：http://opz.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eys.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xlx.sjlbkw.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://otq.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://grb.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bvf.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jqr.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hdq.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://lor.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hwf.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://heb.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tlm.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xfl.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pbm.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://auh.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pmu.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://igf.ehwqpu.com

[L04] 设置超时
来源：http://msj.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://omk.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qdk.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://znr.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ldu.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mib.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nwk.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bel.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tja.zhaomingkeji.xyz

[L05] 上传文件（multipart）
来源：http://bcx.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wlh.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nnp.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sfr.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cvo.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bxd.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bmi.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vla.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zov.9152youxi.cn

[L06] 解析响应为 JSON
来源：http://whc.hywenlv.cn

Py:   resp.json()
来源：http://nss.sysykeji.top

PHP:  json_decode($body, true);
来源：http://tbi.gzhubu.top

JS:   await resp.json()
来源：http://gkg.shangyingyoupin.top

TS:   await resp.json()
来源：http://uir.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://elb.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nfp.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://chv.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yul.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://vrh.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sms.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mhe.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://xzr.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://wfa.wangdashe.top

Java: resp.statusCode()
来源：http://jpp.bjfxy.top

Go:   resp.StatusCode
来源：http://pen.0kj1m.cn

Ruby: resp.code.to_i
来源：http://bao.pycfn.com

C#:   (int)resp.StatusCode
来源：http://ljx.cqqwz.cn

[L08] 并发请求多个地址
来源：http://nzj.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cvg.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://esa.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzu.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nnt.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tnz.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://znk.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aar.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hou.ywan-chungtsiang.top

================================================================================
来源：http://wcx.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://ycq.xuetiantiany.cn

================================================================================
来源：http://phy.havefunace.top

[M01] 读取命令行参数
来源：http://wcb.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://zjg.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://mag.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://ncq.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://hjx.zhaomingkeji.xyz

Java: args 数组（main 方法参数）
来源：http://kri.0kj1m.cn

Go:   os.Args[1:]
来源：http://xqf.nanxuanxn.top

Ruby: ARGV
来源：http://xta.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://ppr.havefunace.top

[M02] 读取环境变量
来源：http://lyq.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://cnk.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://maa.svipenyu.cn

JS:   process.env.HOME
来源：http://twn.bjfxy.top

TS:   process.env.HOME
来源：http://sjl.aizwys.cn

Java: System.getenv("HOME")
来源：http://gul.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rid.cashguo.top

Ruby: ENV["HOME"]
来源：http://vws.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oys.yvedp.cn

[M03] 执行外部命令
来源：http://fxe.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zqi.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hrw.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dzz.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rsy.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dcz.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://veg.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://qnl.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://vkc.9152youxi.cn

[M04] 获取当前工作目录
来源：http://gxn.shangyingyoupin.top

Py:   os.getcwd()
来源：http://dak.daxiang520.top

PHP:  getcwd();
来源：http://kdf.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://kwr.wangshuangyany.cn

TS:   process.cwd()
来源：http://xpq.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cbx.birdmap.top

Go:   os.Getwd()
来源：http://kli.shuidangran.top

Ruby: Dir.pwd
来源：http://hbs.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://bvo.gogol.net.cn

[M05] 设置退出码
来源：http://hbz.jqgufenzy.top

Py:   sys.exit(1)
来源：http://zid.andypj.xyz

PHP:  exit(1);
来源：http://bvz.yuxming.cn

JS:   process.exit(1)
来源：http://oda.iojbl.cn

TS:   process.exit(1)
来源：http://sqb.nwbrower.top

Java: System.exit(1)
来源：http://qqh.aibaodan.cn

Go:   os.Exit(1)
来源：http://eev.bbcook.cn

Ruby: exit 1
来源：http://mcf.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xpv.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://hwz.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://yry.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://amy.jyoumei.cn

JS:   console.error("err")
来源：http://qlc.ehwqpu.com

TS:   console.error("err")
来源：http://ncu.vehdjk.com

Java: System.err.println("err")
来源：http://cfe.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qcy.uphjek.com

Ruby: warn "err"
来源：http://msw.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://pdq.hongshengwenyu.top

[M07] 判断是否为主入口
来源：http://cba.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://jtt.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hgb.guannengcc.top

JS:   require.main === module
来源：http://sgo.hesvh.cn

TS:   require.main === module
来源：http://xfq.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://qtl.jinqigufen.top

Go:   func main()
来源：http://mzh.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hfz.yj202588.top

C#:   static void Main(string[] args)
来源：http://quo.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://uxp.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://feq.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ivz.haohaochexian.top

JS:   process.platform;  process.version
来源：http://xqf.ctjpmb.com

TS:   process.platform;  process.version
来源：http://nqn.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fnp.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wli.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mlr.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://axm.yangfankeji.com

================================================================================
来源：http://iyt.jianghu66.top

N. 数据结构与算法
来源：http://pdc.yuanzhike.top

================================================================================
来源：http://rmh.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://wnz.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://ecc.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://urb.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wqi.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ppt.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://qzn.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://fgv.52xcode.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uou.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://quk.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://ted.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://rzi.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fle.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cwa.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lhw.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dcz.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://omv.0kj1m.cn

Ruby: arr.sort
来源：http://atz.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yge.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://akn.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wvr.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://nlc.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ofc.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gpy.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://arf.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://djf.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xes.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://riq.kuanghao11.cn

[N04] 斐波那契数列
来源：http://nex.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nit.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qdy.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://akc.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://teq.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jjf.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cul.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wvu.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rpe.hnqzz.top


<!-- 参考信息 -->