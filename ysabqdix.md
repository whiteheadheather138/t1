代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://blx.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://ldh.zycfv.cn

Ruby: end - start                 # 返回秒数
来源：http://etc.vqdsnc.cn

C#:   (end - start).TotalSeconds
来源：http://yws.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://mip.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://mhi.shzxlz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kee.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://qhs.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://vcq.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hmt.zhaomingkeji.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jfy.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://jsh.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://wjd.yongpay.top

[J08] 提取年月日与星期
来源：http://wrg.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://esi.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vxi.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fmk.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://glj.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ktg.pycfn.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sdb.0kj1m.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://soj.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tcb.bjfxy.top

[J09] 时区处理
来源：http://ood.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rhh.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ksl.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yxw.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://axb.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://esl.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aif.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://inm.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uqh.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://niz.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yap.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ltr.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://txc.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vwi.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://auv.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hgt.birdmap.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aro.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hmb.jqgufenzy.top

================================================================================
来源：http://aqr.epnwcf.com

K. JSON 与序列化
来源：http://ywz.shuidangran.top

================================================================================
来源：http://mdq.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://hjb.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gjx.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xbt.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://xof.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://ipu.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xsk.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://gmq.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://drt.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hcr.sweek.top

[K02] JSON 字符串转对象
来源：http://feq.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://vic.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pyw.jinqigufen.top

JS:   JSON.parse(s)
来源：http://mgt.dianchejie.cn

TS:   JSON.parse(s)
来源：http://rma.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://crv.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://fql.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://qxk.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rdo.hnxiangtu.top

[K03] JSON 美化输出（带缩进）
来源：http://ctb.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://com.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://itw.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cwd.vehdjk.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ilk.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lmx.zhongyouzk.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hvj.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://guh.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qaf.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://ozg.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gtz.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://omn.yuxming.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mmt.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://itf.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dat.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eyw.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://pgn.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yss.gogol.net.cn

[K05] 深拷贝对象
来源：http://cwe.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://hql.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://spf.c1oappe.top

JS:   structuredClone(obj)
来源：http://iun.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://ryu.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ekl.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wdd.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nyu.pycfn.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ahi.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://bsa.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lqu.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://frx.redwolf501.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xpq.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fod.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wzv.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kqs.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hyk.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pxt.havefunace.top

[K07] 进制转换
来源：http://ata.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jri.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uml.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ife.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iod.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cib.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fxk.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://abe.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://glg.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://aux.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://gyb.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lxt.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://ehc.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://vwp.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ncd.c1oappe.top

Go:   encoding/gob
来源：http://mjw.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://wkd.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fhx.yvedp.cn

================================================================================
来源：http://vbj.hcnkem.com

L. 网络请求
来源：http://ulb.zhiwuduotai.top

================================================================================
来源：http://ihd.316326.xyz

[L01] 发送 GET 请求
来源：http://wmd.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://feg.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oie.uphjek.com

JS:   await fetch(url)
来源：http://vuw.guowangkeji.top

TS:   await fetch(url)
来源：http://bay.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ehn.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://tvc.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wii.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://who.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://vti.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://wyx.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vfi.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eqz.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://itr.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wsk.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mol.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qxe.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wde.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://mfz.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ftu.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ucr.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dof.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zjj.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jar.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sel.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://paa.jinyuanbaomall.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://idu.sxryk.cn

[L04] 设置超时
来源：http://wzo.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://fkq.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://psh.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jmu.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tmz.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xlq.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ndf.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ukt.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vtq.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://vlk.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aho.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qfw.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vev.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dwd.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gac.shuidangran.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ctg.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iom.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://edj.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://lee.yj20258888.top

Py:   resp.json()
来源：http://lvc.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://qis.chenzaomai.com

JS:   await resp.json()
来源：http://qzl.sxryk.cn

TS:   await resp.json()
来源：http://iyv.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dqo.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://caz.hcnkem.com

Ruby: JSON.parse(resp.body)
来源：http://zhz.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ysl.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://quy.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://atq.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ynf.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://hom.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://kbl.kuanghao11.cn

Java: resp.statusCode()
来源：http://vzb.hywenlv.cn

Go:   resp.StatusCode
来源：http://oba.hnqzz.top

Ruby: resp.code.to_i
来源：http://zvd.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://hwm.meibo888.top

[L08] 并发请求多个地址
来源：http://qja.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tbe.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://zps.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wbh.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cjb.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xpt.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xsu.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ahi.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kjv.fzhhl.top

================================================================================
来源：http://eqc.hywenlv.cn

M. 命令行 / 进程 / 环境
来源：http://jin.ywan-chungtsiang.top

================================================================================
来源：http://ezt.meibo888.top

[M01] 读取命令行参数
来源：http://zun.hesvh.cn

Py:   sys.argv[1:]
来源：http://fen.bjfxy.top

PHP:  $argv;  $argc;
来源：http://tgl.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://qdq.sxryk.cn

TS:   process.argv.slice(2)
来源：http://kba.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://msp.snrcjt.cn

Go:   os.Args[1:]
来源：http://frs.jqgfzy.top

Ruby: ARGV
来源：http://uyo.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://rqa.uphjek.com

[M02] 读取环境变量
来源：http://quu.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://dgs.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wdc.yvedp.cn

JS:   process.env.HOME
来源：http://vvf.hongshengwenyu.top

TS:   process.env.HOME
来源：http://rpr.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://mmb.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cmv.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://sas.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://miy.hfpthk.cn

[M03] 执行外部命令
来源：http://efq.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vpp.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rfj.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://haz.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://gzp.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ffc.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://pqt.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://oyg.sweek.top

C#:   Process.Start("ls", "-l");
来源：http://bmp.zdqjudy.top

[M04] 获取当前工作目录
来源：http://fak.chenjidiqi.icu

Py:   os.getcwd()
来源：http://rdr.cdnleiting.top

PHP:  getcwd();
来源：http://asm.hywenlv.cn

JS:   process.cwd()
来源：http://pmc.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://vze.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://nie.0kj1m.cn

Go:   os.Getwd()
来源：http://dgq.dashuyun.cn

Ruby: Dir.pwd
来源：http://zjn.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://vvq.zhoulong.xyz

[M05] 设置退出码
来源：http://gau.kuanghao11.cn

Py:   sys.exit(1)
来源：http://owm.guannengcc.top

PHP:  exit(1);
来源：http://pfh.haohaochexian.top

JS:   process.exit(1)
来源：http://fgz.pengpengdd.cyou

TS:   process.exit(1)
来源：http://rek.wangdashe.top

Java: System.exit(1)
来源：http://fvw.jlsjyb.cn

Go:   os.Exit(1)
来源：http://arw.hammf.cn

Ruby: exit 1
来源：http://hsc.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fuy.zhoulong.xyz

[M06] 向标准错误输出
来源：http://rvt.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://fvh.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oxs.316326.xyz

JS:   console.error("err")
来源：http://rpa.yanxiufei.cn

TS:   console.error("err")
来源：http://pdu.hfpthk.cn

Java: System.err.println("err")
来源：http://pjo.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://txh.gzhubu.top

Ruby: warn "err"
来源：http://rky.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://uya.zycfv.cn

[M07] 判断是否为主入口
来源：http://bwh.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://zkb.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xuq.havefunace.top

JS:   require.main === module
来源：http://bph.ydzc1.top

TS:   require.main === module
来源：http://qbi.xuanzx.com

Java: public static void main(String[] args)
来源：http://iut.yvedp.cn

Go:   func main()
来源：http://iod.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nge.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://gbl.tarul.cn

[M08] 获取系统与运行时信息
来源：http://wdu.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://kti.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://owx.guowangkeji.top

JS:   process.platform;  process.version
来源：http://ibm.jiagoushi.top

TS:   process.platform;  process.version
来源：http://gbp.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://myv.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://orv.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rtx.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qls.yfazqb.com

================================================================================
来源：http://qnx.sjlbkw.cn

N. 数据结构与算法
来源：http://wku.birdmap.top

================================================================================
来源：http://fbm.havefunace.top

[N01] 二分查找（有序数组）
来源：http://jjd.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://qyz.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fji.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xbb.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zhh.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://dce.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://bdl.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://flu.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://wcd.jyoumei.cn

[N02] 排序（工程实践用内置实现）
来源：http://frr.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://yox.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ydd.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://dbu.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://akv.zhaomingkeji.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://huz.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://lhx.ybcxt.top

Ruby: arr.sort
来源：http://cbb.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://obn.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://hyr.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://spf.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://ctw.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://znz.fktsv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rde.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nij.tanke756.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://elj.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://glo.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ohi.cashguo.top

[N04] 斐波那契数列
来源：http://oye.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tpd.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zkp.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://npb.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hib.yuxming.cn


<!-- 参考信息 -->