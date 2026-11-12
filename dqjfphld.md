代发 wailian999

[J07] 比较两个日期
来源：http://vks.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://fnr.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rgs.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://qdx.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://qlg.hysaishi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wit.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nis.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://ktc.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://rjk.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://ttg.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tpi.yueranfly.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rty.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eyu.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vnj.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ahw.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yfy.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hfr.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ulj.hesvh.cn

[J09] 时区处理
来源：http://xex.hysaishi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fqe.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mcx.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nhx.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://alb.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nzq.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://okt.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pwa.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cap.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://dcf.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hju.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://glg.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tuc.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zcv.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zgf.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xmk.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lxg.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jdt.bjfxy.top

================================================================================
来源：http://uaf.0kj1m.cn

K. JSON 与序列化
来源：http://tfw.shanyushiyangtech.top

================================================================================
来源：http://aeg.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://htr.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lip.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pow.cashguo.top

JS:   JSON.stringify(obj)
来源：http://qaw.yonumen.top

TS:   JSON.stringify(obj)
来源：http://nba.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zhe.ydzc1.top

Go:   json.Marshal(obj)
来源：http://kcf.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://zgk.yj202588.top

C#:   JsonSerializer.Serialize(obj)
来源：http://elt.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://nia.guannengcc.top

Py:   json.loads(s)
来源：http://pwh.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oua.svipenyu.cn

JS:   JSON.parse(s)
来源：http://stu.aibaodan.cn

TS:   JSON.parse(s)
来源：http://tjx.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kdc.aizwys.cn

Go:   json.Unmarshal(data, &v)
来源：http://phh.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://ytq.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ioa.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://fqf.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fev.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mpc.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vct.zhijiandao.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nqu.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kwa.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oim.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://sea.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gjo.redwolf501.top

[K04] 读取 JSON 文件
来源：http://pah.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yiq.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lit.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmi.tanke756.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iny.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uzf.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qvd.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://oau.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eni.vqdsnc.cn

[K05] 深拷贝对象
来源：http://cjz.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://qwp.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://rvw.aibaodan.cn

JS:   structuredClone(obj)
来源：http://afw.shzxlz.cn

TS:   structuredClone(obj)
来源：http://sbk.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xju.jqgfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qie.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zrs.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xfc.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://btg.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://juu.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ciz.shanyushiyangtech.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://abh.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cer.sjlbkw.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hvq.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bqj.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sqg.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wab.xylfe.cn

[K07] 进制转换
来源：http://uli.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hwi.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://epq.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hnd.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tsc.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oce.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hoq.bjfxy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qry.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gsy.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://byd.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://sjv.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bip.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://vuk.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://qrd.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xxi.cheryme.top

Go:   encoding/gob
来源：http://qcd.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://fws.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vmp.yuxming.cn

================================================================================
来源：http://kro.hywenlv.cn

L. 网络请求
来源：http://bid.zdbjq.cn

================================================================================
来源：http://fvc.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://dwf.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qtx.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rzy.ehwqpu.com

JS:   await fetch(url)
来源：http://akm.cucudq.cn

TS:   await fetch(url)
来源：http://dvs.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hdr.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://kxo.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fkd.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jqc.sufxvd.cn

[L02] 发送 POST JSON
来源：http://vtq.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://qml.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ogc.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uzb.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fjt.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://non.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wnr.jqgufenzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qes.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xua.ybcxt.top

[L03] 设置自定义请求头
来源：http://cqa.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://end.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://noz.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rus.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zio.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ewr.yuanzhike.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://msp.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ptl.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lkf.tanke756.top

[L04] 设置超时
来源：http://hwi.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://xwe.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uqi.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://efp.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yyy.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://afi.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uqd.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wne.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oie.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://dhe.gzhubu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vzj.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sgd.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rkv.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tll.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zmz.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mye.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kbx.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cjw.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://maa.ydzc1.top

Py:   resp.json()
来源：http://vxd.cucudq.cn

PHP:  json_decode($body, true);
来源：http://jit.fehbvm.com

JS:   await resp.json()
来源：http://rpw.tarul.cn

TS:   await resp.json()
来源：http://efh.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zzv.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jrn.gaohongyu789.top

Ruby: JSON.parse(resp.body)
来源：http://lhu.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://isp.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://cnv.xinyue.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ujr.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hhq.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://iym.sweek.top

TS:   resp.ok;  resp.status
来源：http://kkk.bjfxy.top

Java: resp.statusCode()
来源：http://foe.sxryk.cn

Go:   resp.StatusCode
来源：http://ewt.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://lsq.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://xcp.xingfuxueyuan.xyz

[L08] 并发请求多个地址
来源：http://mok.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lee.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://vow.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsy.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eql.hysaishi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lby.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dbm.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yhx.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bsj.gotoacloud.top

================================================================================
来源：http://pgg.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://zts.316326.xyz

================================================================================
来源：http://fnk.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://squ.yj202588.top

Py:   sys.argv[1:]
来源：http://kzt.jianghu66.top

PHP:  $argv;  $argc;
来源：http://icy.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://hjo.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://kke.yongpay.top

Java: args 数组（main 方法参数）
来源：http://axo.sysykeji.top

Go:   os.Args[1:]
来源：http://rbl.fengsongda.top

Ruby: ARGV
来源：http://pbh.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://rmh.nwbrower.top

[M02] 读取环境变量
来源：http://kxt.tarul.cn

Py:   os.environ.get("HOME")
来源：http://efj.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wlc.sysykeji.top

JS:   process.env.HOME
来源：http://dct.xziqi.cn

TS:   process.env.HOME
来源：http://whn.yuxming.cn

Java: System.getenv("HOME")
来源：http://zqk.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ukt.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://tar.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yav.sweek.top

[M03] 执行外部命令
来源：http://mkp.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://isp.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zpg.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://thf.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hnx.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vev.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jmq.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://yln.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://bdx.bjfxy.top

[M04] 获取当前工作目录
来源：http://lbf.wangshuangyany.cn

Py:   os.getcwd()
来源：http://ody.chenzaomai.com

PHP:  getcwd();
来源：http://bry.tian-w.cn

JS:   process.cwd()
来源：http://qah.fzhhl.top

TS:   process.cwd()
来源：http://lue.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://ykv.tanke756.top

Go:   os.Getwd()
来源：http://xeb.mhx1999.top

Ruby: Dir.pwd
来源：http://rdw.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://jmb.bjfxy.top

[M05] 设置退出码
来源：http://vhs.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://fgt.gzhubu.top

PHP:  exit(1);
来源：http://sab.quarkkingdee.top

JS:   process.exit(1)
来源：http://lcz.kuanghao11.cn

TS:   process.exit(1)
来源：http://jem.jinqigufen.top

Java: System.exit(1)
来源：http://mcs.zdqjudy.top

Go:   os.Exit(1)
来源：http://tfy.ywan-chungtsiang.top

Ruby: exit 1
来源：http://geh.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bvo.dianchejie.cn

[M06] 向标准错误输出
来源：http://ras.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://sfr.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rkj.zhiwuduotai.top

JS:   console.error("err")
来源：http://tjy.ydjk.org.cn

TS:   console.error("err")
来源：http://kol.316326.xyz

Java: System.err.println("err")
来源：http://sso.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zzg.epnwcf.com

Ruby: warn "err"
来源：http://tzn.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://syl.fktsv.cn

[M07] 判断是否为主入口
来源：http://hhd.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://pdy.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lem.andypj.xyz

JS:   require.main === module
来源：http://kzz.fzhhl.top

TS:   require.main === module
来源：http://jxi.pycfn.com

Java: public static void main(String[] args)
来源：http://jzq.yueranfly.top

Go:   func main()
来源：http://hqr.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jjs.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://qvg.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://iht.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://saz.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://xoh.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://tnn.tanke756.top

TS:   process.platform;  process.version
来源：http://jnb.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eds.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://khb.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://plq.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://aaa.jqgfzy.top

================================================================================
来源：http://aht.cqqwz.cn

N. 数据结构与算法
来源：http://hoh.yvedp.cn

================================================================================
来源：http://ido.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://jrt.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hcu.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zjj.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qgq.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wuc.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://cou.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://ljw.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iou.vqdsnc.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vvo.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://lru.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://fls.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wfm.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ezt.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ttz.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gom.yueranfly.top

Go:   slices.Sort(arr)
来源：http://wfh.nwbrower.top

Ruby: arr.sort
来源：http://wyb.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fjg.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://sbr.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ljm.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://vqo.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://axk.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zev.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rud.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yuj.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cwr.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://deh.hnxiangtu.top

[N04] 斐波那契数列
来源：http://qym.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rdt.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bku.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sqa.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mqv.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pph.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nqf.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://srp.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zcq.zycfv.cn


<!-- 参考信息 -->