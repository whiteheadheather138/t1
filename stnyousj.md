代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jgx.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://zce.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://tqa.vqdsnc.cn

[J06] 计算两时间之差
来源：http://jbd.tarul.cn

Py:   (end - start).total_seconds()
来源：http://wma.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://klw.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ipd.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bsw.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hfc.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://bal.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://pjj.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://wkm.fktsv.cn

[J07] 比较两个日期
来源：http://gte.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://wmm.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fxy.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://dzk.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://dkg.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zxc.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gdt.cdnleiting.top

Ruby: d1 < d2;  d1 == d2
来源：http://lru.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://ngf.aibaodan.cn

[J08] 提取年月日与星期
来源：http://pee.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://led.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yfg.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cgc.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dwn.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ksy.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tas.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lzb.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xoe.jinghuilouyu.cn

[J09] 时区处理
来源：http://jzm.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pey.yueranfly.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nmo.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxk.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kls.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://brc.jiagoushi.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cte.ehwqpu.com

Ruby: Time.now.getlocal("+08:00")
来源：http://qbk.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zsk.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://gaf.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://skx.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://inv.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fjy.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nnv.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mxa.smart0.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jnv.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qtu.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kwh.yvedp.cn

================================================================================
来源：http://sog.cucudq.cn

K. JSON 与序列化
来源：http://uhi.yfazqb.com

================================================================================
来源：http://xoj.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://ibi.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://emd.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cou.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://rdl.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://avw.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rae.c1oappe.top

Go:   json.Marshal(obj)
来源：http://qda.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://fxo.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rem.cashguo.top

[K02] JSON 字符串转对象
来源：http://yqc.daria6918.cn

Py:   json.loads(s)
来源：http://kxv.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dpl.smart0.xyz

JS:   JSON.parse(s)
来源：http://olr.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://fqm.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://epx.yueranfly.top

Go:   json.Unmarshal(data, &v)
来源：http://lsv.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://kjc.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zzt.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://lfq.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fnb.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xim.sysykeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kwr.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gur.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jym.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zuq.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gsr.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wtc.andypj.xyz

[K04] 读取 JSON 文件
来源：http://rob.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://laq.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nxs.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://utp.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rxe.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lws.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qrm.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://umg.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rvi.zhijiandao.cn

[K05] 深拷贝对象
来源：http://lsx.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://diu.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://dxf.jiagoushi.top

JS:   structuredClone(obj)
来源：http://eqt.yonumen.top

TS:   structuredClone(obj)
来源：http://cez.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sxk.dianchejie.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jwk.yj20258.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kvc.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fwm.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://wne.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fyr.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://svq.daria6918.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kil.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://awu.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wgw.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jni.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tfp.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cxu.0kj1m.cn

[K07] 进制转换
来源：http://cqe.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iry.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bck.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://efc.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ixt.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fit.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kyw.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xpr.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gil.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://qbz.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://wnp.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jcr.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://osq.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://tnf.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://srz.yuanzhike.top

Go:   encoding/gob
来源：http://fho.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://mpo.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nrv.jiagoushi.top

================================================================================
来源：http://mnj.yvedp.cn

L. 网络请求
来源：http://qlv.feifeiyinyue.top

================================================================================
来源：http://ffe.xuanzx.com

[L01] 发送 GET 请求
来源：http://ckz.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ecy.pycfn.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jbx.kuanghao11.cn

JS:   await fetch(url)
来源：http://xfb.tianlin.xyz

TS:   await fetch(url)
来源：http://obu.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gth.zdqjudy.top

Go:   resp, err := http.Get(url)
来源：http://hus.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hjy.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mpz.nanxinkj.top

[L02] 发送 POST JSON
来源：http://pjo.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://hxj.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xkc.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mnv.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dge.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gdw.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jsa.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bjb.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ehi.sufxvd.cn

[L03] 设置自定义请求头
来源：http://gvj.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oqx.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://osk.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vux.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://luf.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://khf.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mde.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vtp.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ncs.hammf.cn

[L04] 设置超时
来源：http://iko.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://iyx.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gyi.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ywf.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zcb.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hqf.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kys.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ref.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fsh.aizwys.cn

[L05] 上传文件（multipart）
来源：http://ndj.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xno.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ecn.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zqa.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vau.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vxg.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ikr.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yca.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ges.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://svv.hnxiangtu.top

Py:   resp.json()
来源：http://msg.tanke756.top

PHP:  json_decode($body, true);
来源：http://nzl.ehwqpu.com

JS:   await resp.json()
来源：http://vyk.yuanzhike.top

TS:   await resp.json()
来源：http://dfh.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iit.zhijiandao.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lag.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://jev.chenzaomai.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://izd.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://onb.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lvy.shanyushiyangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ogi.pycfn.com

JS:   resp.ok;  resp.status
来源：http://xlg.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://ojo.zdbjq.cn

Java: resp.statusCode()
来源：http://apf.ppjwa.cn

Go:   resp.StatusCode
来源：http://ahh.xinyue.icu

Ruby: resp.code.to_i
来源：http://qec.cashguo.top

C#:   (int)resp.StatusCode
来源：http://hzz.cqqwz.cn

[L08] 并发请求多个地址
来源：http://duk.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yjg.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://ukr.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hkp.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mss.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ldi.xylfe.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fbi.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xfu.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ocq.feifeiyinyue.top

================================================================================
来源：http://acl.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://uns.yueranfly.top

================================================================================
来源：http://waz.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://mwd.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://bdl.pycfn.com

PHP:  $argv;  $argc;
来源：http://pvr.sweek.top

JS:   process.argv.slice(2)
来源：http://kbq.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://udc.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://vlr.zdbjq.cn

Go:   os.Args[1:]
来源：http://zkh.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://trg.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://khe.xziqi.cn

[M02] 读取环境变量
来源：http://xrj.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://bsx.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ehu.sxryk.cn

JS:   process.env.HOME
来源：http://zvg.ybcxt.top

TS:   process.env.HOME
来源：http://znh.bjfxy.top

Java: System.getenv("HOME")
来源：http://zmg.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fre.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://oon.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sfc.aizwys.cn

[M03] 执行外部命令
来源：http://ztq.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wzv.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mtm.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://enx.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kfo.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wpw.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://drd.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://lft.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://pbe.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://dgb.gotoacloud.top

Py:   os.getcwd()
来源：http://bdx.ydjk.org.cn

PHP:  getcwd();
来源：http://esp.ydzc1.top

JS:   process.cwd()
来源：http://hxz.ybcxt.top

TS:   process.cwd()
来源：http://lai.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://tew.wangshuangyany.cn

Go:   os.Getwd()
来源：http://qwa.gaohongyu789.top

Ruby: Dir.pwd
来源：http://hvu.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://qje.chenzaomai.com

[M05] 设置退出码
来源：http://zes.gogol.net.cn

Py:   sys.exit(1)
来源：http://tpf.aizwys.cn

PHP:  exit(1);
来源：http://pmr.vqdsnc.cn

JS:   process.exit(1)
来源：http://brz.jyoumei.cn

TS:   process.exit(1)
来源：http://sho.gaohongyu789.top

Java: System.exit(1)
来源：http://mpl.epnwcf.com

Go:   os.Exit(1)
来源：http://yjh.jinqigfzy.top

Ruby: exit 1
来源：http://scx.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://egy.zdbjq.cn

[M06] 向标准错误输出
来源：http://yba.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://fvy.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wsy.jqgufenzy.top

JS:   console.error("err")
来源：http://cob.jinqigfzy.top

TS:   console.error("err")
来源：http://dqs.yfazqb.com

Java: System.err.println("err")
来源：http://trx.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tli.bbcook.cn

Ruby: warn "err"
来源：http://fmi.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://xxn.haohaochexian.top

[M07] 判断是否为主入口
来源：http://xao.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://fgo.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iyx.hysaishi.cn

JS:   require.main === module
来源：http://wxo.aibaodan.cn

TS:   require.main === module
来源：http://ryt.xziqi.cn

Java: public static void main(String[] args)
来源：http://fsf.yfazqb.com

Go:   func main()
来源：http://mvz.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tcz.yuxming.cn

C#:   static void Main(string[] args)
来源：http://ndz.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://fio.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://agj.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://xgj.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://esy.epnwcf.com

TS:   process.platform;  process.version
来源：http://mxy.guannengcc.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lvt.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fqg.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cqy.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://gir.aizwys.cn

================================================================================
来源：http://imr.jianghu66.top

N. 数据结构与算法
来源：http://yrp.jinqigufen.top

================================================================================
来源：http://sun.zhoulong.xyz

[N01] 二分查找（有序数组）
来源：http://sam.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nxh.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ddu.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gcl.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xrp.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ydy.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://veq.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rth.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://aed.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://oyc.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://cnh.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pii.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eul.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://qts.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hcj.svipenyu.cn

Go:   slices.Sort(arr)
来源：http://phf.quarkkingdee.top

Ruby: arr.sort
来源：http://ici.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ogt.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://ttr.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://doh.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://jph.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pqq.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vlc.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ufk.shuidangran.top


<!-- 参考信息 -->