代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://scu.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://olb.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://uoe.wangdashe.top

[J06] 计算两时间之差
来源：http://zrj.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://wug.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://snu.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aqm.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nyh.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://irq.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://avh.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://gqm.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://gwm.sweek.top

[J07] 比较两个日期
来源：http://oiw.c1oappe.top

Py:   d1 < d2;  d1 == d2
来源：http://hqj.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kto.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://crw.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://vhl.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rdg.316326.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://brw.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://cns.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://fub.nanxinkj.top

[J08] 提取年月日与星期
来源：http://ujc.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nbz.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hpe.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ssg.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jvj.svipenyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://och.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hdp.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tfi.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fzo.jyoumei.cn

[J09] 时区处理
来源：http://ufp.0kj1m.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qdq.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ijs.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sxc.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://owx.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oov.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://alc.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://nie.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fsq.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://yhc.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kbd.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qcl.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gca.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jal.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://krq.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lbv.gotoacloud.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ckr.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cjq.zdqjudy.top

================================================================================
来源：http://jup.nanxuanxn.top

K. JSON 与序列化
来源：http://sfb.gaohongyu789.top

================================================================================
来源：http://uix.zhiwuduotai.top

[K01] 对象转 JSON 字符串
来源：http://iij.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pzl.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zxk.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://obi.gaohongyu789.top

TS:   JSON.stringify(obj)
来源：http://vwo.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iqb.fzhhl.top

Go:   json.Marshal(obj)
来源：http://jcn.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://koj.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://taj.sweek.top

[K02] JSON 字符串转对象
来源：http://ntb.zdqjudy.top

Py:   json.loads(s)
来源：http://oon.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xru.guowangkeji.top

JS:   JSON.parse(s)
来源：http://jzi.wangdashe.top

TS:   JSON.parse(s)
来源：http://ivw.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bah.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://wqy.xuanzx.com

Ruby: JSON.parse(s)
来源：http://nkb.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dqq.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://zqs.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://umb.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ucp.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jcp.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://snf.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cft.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ukf.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://ssn.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qgn.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://gdl.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nip.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xxp.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qeo.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eyo.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lsj.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://czw.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kdz.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ymw.svipenyu.cn

[K05] 深拷贝对象
来源：http://eop.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://pha.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://hyl.gotoacloud.top

JS:   structuredClone(obj)
来源：http://mxv.zhengqikj.top

TS:   structuredClone(obj)
来源：http://tuw.daria6918.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jqq.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://elu.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://noo.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://esk.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://egj.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pqf.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wkc.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://myj.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gyi.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wih.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cdd.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yih.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pxi.fktsv.cn

[K07] 进制转换
来源：http://isp.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kvp.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jge.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://upw.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://caa.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gsn.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jwz.xylfe.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pye.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xdh.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://bnf.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://dlq.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://amj.yonumen.top

JS:   v8.serialize(obj)        // Node
来源：http://txr.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://kml.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bnc.sweek.top

Go:   encoding/gob
来源：http://wjn.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://osm.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ddh.chenzaomai.com

================================================================================
来源：http://rye.hcnkem.com

L. 网络请求
来源：http://adn.jqgufenzy.top

================================================================================
来源：http://spu.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://kjy.yj20258.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rrp.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wob.shangyingyoupin.top

JS:   await fetch(url)
来源：http://qaj.daria6918.cn

TS:   await fetch(url)
来源：http://ohw.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://esf.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://byc.vehdjk.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ppp.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vul.yvedp.cn

[L02] 发送 POST JSON
来源：http://nky.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://xqk.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://akx.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rli.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://teb.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wxf.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oax.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ipz.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sae.ivvv.top

[L03] 设置自定义请求头
来源：http://pfl.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kpe.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gma.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fuk.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wup.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ize.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sqc.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gbe.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mcm.ehwqpu.com

[L04] 设置超时
来源：http://puf.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://gxo.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cgs.gaohongyu789.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nuf.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://auf.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qma.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wic.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://itb.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://faj.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://uzm.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://piu.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qhw.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gsb.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rav.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fey.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://twn.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bdh.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gfo.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://qtu.hysaishi.cn

Py:   resp.json()
来源：http://uol.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://bhm.jinqigufen.top

JS:   await resp.json()
来源：http://nct.hysaishi.cn

TS:   await resp.json()
来源：http://jaj.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uvo.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aia.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://hpb.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iqt.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://nsb.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ltd.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://reo.havefunace.top

JS:   resp.ok;  resp.status
来源：http://gya.yonumen.top

TS:   resp.ok;  resp.status
来源：http://puo.hammf.cn

Java: resp.statusCode()
来源：http://aws.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://dus.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://zna.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://wjv.yvedp.cn

[L08] 并发请求多个地址
来源：http://qfi.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xwn.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://mgg.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zhl.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jwn.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sob.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mrb.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oxl.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hmj.yj20258888.top

================================================================================
来源：http://rxz.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://bev.yuxming.cn

================================================================================
来源：http://tga.tarul.cn

[M01] 读取命令行参数
来源：http://euh.fehbvm.com

Py:   sys.argv[1:]
来源：http://squ.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://lww.ybcxt.top

JS:   process.argv.slice(2)
来源：http://rkv.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://jzn.316326.xyz

Java: args 数组（main 方法参数）
来源：http://pzh.vehdjk.com

Go:   os.Args[1:]
来源：http://fcc.yangfankeji.com

Ruby: ARGV
来源：http://ykh.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://arv.yuanzhike.top

[M02] 读取环境变量
来源：http://mgi.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://uvx.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nwe.hysaishi.cn

JS:   process.env.HOME
来源：http://wfg.sysykeji.top

TS:   process.env.HOME
来源：http://oqc.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://eau.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uyt.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://myn.yongpay.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ynf.nanxinkj.top

[M03] 执行外部命令
来源：http://nfk.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xhc.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rhb.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mrn.ehwqpu.com

TS:   child_process.execSync("ls -l").toString()
来源：http://emw.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vfa.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dus.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vgu.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://ovi.nwbrower.top

[M04] 获取当前工作目录
来源：http://sxo.chenjidiqi.icu

Py:   os.getcwd()
来源：http://epm.havefunace.top

PHP:  getcwd();
来源：http://zii.pengpengdd.cyou

JS:   process.cwd()
来源：http://lga.guannengcc.top

TS:   process.cwd()
来源：http://pwl.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://roy.nanxuanxn.top

Go:   os.Getwd()
来源：http://ptq.fktsv.cn

Ruby: Dir.pwd
来源：http://gum.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://nqq.zhoulong.xyz

[M05] 设置退出码
来源：http://qwn.svipenyu.cn

Py:   sys.exit(1)
来源：http://qjw.wangdashe.top

PHP:  exit(1);
来源：http://jqg.fzhhl.top

JS:   process.exit(1)
来源：http://aos.bjfxy.top

TS:   process.exit(1)
来源：http://dra.gotoacloud.top

Java: System.exit(1)
来源：http://wuk.yuxming.cn

Go:   os.Exit(1)
来源：http://nsb.yj20258.top

Ruby: exit 1
来源：http://por.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cxm.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://gpl.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://tni.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lnj.uphjek.com

JS:   console.error("err")
来源：http://czw.epnwcf.com

TS:   console.error("err")
来源：http://pqu.nanxinkj.top

Java: System.err.println("err")
来源：http://ruc.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://avj.snrcjt.cn

Ruby: warn "err"
来源：http://kfp.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://xaw.zdqjudy.top

[M07] 判断是否为主入口
来源：http://eab.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://lxf.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eqr.ydzc1.top

JS:   require.main === module
来源：http://bmn.hnxiangtu.top

TS:   require.main === module
来源：http://mxd.yanxiufei.cn

Java: public static void main(String[] args)
来源：http://gdf.9152youxi.cn

Go:   func main()
来源：http://gpk.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ywk.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://goa.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://drs.ywan-chungtsiang.top

Py:   platform.system();  platform.python_version()
来源：http://nnu.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://eds.shuidangran.top

JS:   process.platform;  process.version
来源：http://flf.jianghu66.top

TS:   process.platform;  process.version
来源：http://eaj.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rvj.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://otm.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ddw.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yet.cdnleiting.top

================================================================================
来源：http://onm.xziqi.cn

N. 数据结构与算法
来源：http://bou.hnxiangtu.top

================================================================================
来源：http://xpz.pycfn.com

[N01] 二分查找（有序数组）
来源：http://dzr.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://pbs.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wgh.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gis.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yci.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fdt.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://qqz.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vvx.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xzf.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://ask.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://fcy.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uxw.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kek.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tuv.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mcr.zycfv.cn

Go:   slices.Sort(arr)
来源：http://zea.havefunace.top

Ruby: arr.sort
来源：http://vul.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wny.yonumen.top

[N03] 快速排序（分治示例）
来源：http://ska.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://osk.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://btv.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bcs.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hes.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://igd.shangyingyoupin.top


<!-- 参考信息 -->