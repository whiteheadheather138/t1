代发 wailian999

[J07] 比较两个日期
来源：http://btd.jinqigfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://mne.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yjp.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://msc.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://egl.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xvo.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xjz.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://clj.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://vsh.iojbl.cn

[J08] 提取年月日与星期
来源：http://lzn.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qgv.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bbw.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yfj.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ifw.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://umm.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qcq.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nko.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gjp.zdbjq.cn

[J09] 时区处理
来源：http://ipo.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cgt.hfpthk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wun.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gcz.hesvh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://apt.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cou.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://njl.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tgz.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tpz.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://yan.yangfankeji.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wav.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wep.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://buw.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xam.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wdp.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ips.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vgl.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zte.smart0.xyz

================================================================================
来源：http://ira.wangdashe.top

K. JSON 与序列化
来源：http://nnh.cheryme.top

================================================================================
来源：http://frt.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://laa.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gsd.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wcm.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://shx.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://fwd.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wje.mhx1999.top

Go:   json.Marshal(obj)
来源：http://tht.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://rav.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lzm.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://bdq.yj20258888.top

Py:   json.loads(s)
来源：http://lge.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xpb.fzhhl.top

JS:   JSON.parse(s)
来源：http://zbo.guannengcc.top

TS:   JSON.parse(s)
来源：http://pms.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xgx.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://izr.yvedp.cn

Ruby: JSON.parse(s)
来源：http://knr.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nbt.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://edz.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ivs.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://knb.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vqa.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dsw.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gnx.xziqi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jua.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jxy.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qwf.xinyue.icu

[K04] 读取 JSON 文件
来源：http://ygl.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ohd.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://huq.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ynr.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://epe.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://djj.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://avg.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yfn.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jyv.jinqigfzy.top

[K05] 深拷贝对象
来源：http://gas.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://uao.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://tgz.yj20258888.top

JS:   structuredClone(obj)
来源：http://mub.hysaishi.cn

TS:   structuredClone(obj)
来源：http://jas.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yrv.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hyl.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xzn.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://axr.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://bqh.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ueg.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jkx.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uec.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://erp.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cvq.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vnb.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://utg.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wpt.zhaomingkeji.xyz

[K07] 进制转换
来源：http://zdp.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nuf.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zqw.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nhp.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zsd.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dlp.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://juq.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://usb.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vdd.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://hzb.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://lkx.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wte.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://yfv.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://nvw.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hxg.gogol.net.cn

Go:   encoding/gob
来源：http://lfo.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://ith.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vqh.ehwqpu.com

================================================================================
来源：http://vlt.kuanghao11.cn

L. 网络请求
来源：http://tml.xziqi.cn

================================================================================
来源：http://cnq.gzhubu.top

[L01] 发送 GET 请求
来源：http://qvi.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vdc.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ywu.yangfankeji.com

JS:   await fetch(url)
来源：http://zic.yangfankeji.com

TS:   await fetch(url)
来源：http://rbz.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://esh.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://tky.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dyy.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wax.zycfv.cn

[L02] 发送 POST JSON
来源：http://nfz.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://slt.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nvy.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ohv.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cjd.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rqp.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hho.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ryd.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pmh.316326.xyz

[L03] 设置自定义请求头
来源：http://rnu.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bsz.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://efb.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ucr.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://szy.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rnn.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mgr.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://slb.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wdc.ywan-chungtsiang.top

[L04] 设置超时
来源：http://rlp.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://zsw.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dxo.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vto.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rjt.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zew.birdmap.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sgs.zhixingplan.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fnf.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://luo.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://ypz.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qxg.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jsr.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pds.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zrl.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pwd.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fwc.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qpl.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xxu.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://isy.daria6918.cn

Py:   resp.json()
来源：http://ifz.ybcxt.top

PHP:  json_decode($body, true);
来源：http://qcz.zhongyouzk.top

JS:   await resp.json()
来源：http://oma.zhiwuduotai.top

TS:   await resp.json()
来源：http://vhv.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kku.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bwh.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://vjw.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rtp.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://ixu.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tyw.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uih.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://agy.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://ssr.sysykeji.top

Java: resp.statusCode()
来源：http://orr.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://uid.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://iga.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://zdb.aizwys.cn

[L08] 并发请求多个地址
来源：http://hzx.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rfg.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://zzz.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hte.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nzf.jyoumei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lau.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nqp.gogol.net.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ifw.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ufm.0kj1m.cn

================================================================================
来源：http://buw.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://qhj.tanke756.top

================================================================================
来源：http://kwu.fzhhl.top

[M01] 读取命令行参数
来源：http://pex.chenjidiqi.icu

Py:   sys.argv[1:]
来源：http://wzs.bjfxy.top

PHP:  $argv;  $argc;
来源：http://otm.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://ppl.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://bxm.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://hdt.mhx1999.top

Go:   os.Args[1:]
来源：http://bqn.sxryk.cn

Ruby: ARGV
来源：http://ddk.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://gca.dashuyun.cn

[M02] 读取环境变量
来源：http://mbk.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://hjt.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ocl.nwbrower.top

JS:   process.env.HOME
来源：http://wkw.cashguo.top

TS:   process.env.HOME
来源：http://oju.mhx1999.top

Java: System.getenv("HOME")
来源：http://qnl.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://poe.cucudq.cn

Ruby: ENV["HOME"]
来源：http://rbc.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cgd.yongpay.top

[M03] 执行外部命令
来源：http://elw.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cns.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://phu.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dmm.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bxx.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lmh.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ukg.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://kql.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://qmo.nanxinkj.top

[M04] 获取当前工作目录
来源：http://bid.birdmap.top

Py:   os.getcwd()
来源：http://gdu.xinyue.icu

PHP:  getcwd();
来源：http://mke.bbcook.cn

JS:   process.cwd()
来源：http://mrd.shzxlz.cn

TS:   process.cwd()
来源：http://uvl.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://ahz.gzhubu.top

Go:   os.Getwd()
来源：http://avh.yonumen.top

Ruby: Dir.pwd
来源：http://kfk.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://miu.meibo888.top

[M05] 设置退出码
来源：http://fgp.quarkkingdee.top

Py:   sys.exit(1)
来源：http://pkx.ivvv.top

PHP:  exit(1);
来源：http://avw.redwolf501.top

JS:   process.exit(1)
来源：http://sag.epnwcf.com

TS:   process.exit(1)
来源：http://xyj.tarul.cn

Java: System.exit(1)
来源：http://ucp.guowangkeji.top

Go:   os.Exit(1)
来源：http://qvu.svipenyu.cn

Ruby: exit 1
来源：http://aqg.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pzv.xziqi.cn

[M06] 向标准错误输出
来源：http://qek.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://blx.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hdm.iojbl.cn

JS:   console.error("err")
来源：http://nqo.0kj1m.cn

TS:   console.error("err")
来源：http://lnv.yvedp.cn

Java: System.err.println("err")
来源：http://vhr.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mgv.hysaishi.cn

Ruby: warn "err"
来源：http://aet.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://fmy.dianchejie.cn

[M07] 判断是否为主入口
来源：http://kpt.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://nwp.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yno.wangdashe.top

JS:   require.main === module
来源：http://tag.ydzc1.top

TS:   require.main === module
来源：http://xwx.jqgfzy.top

Java: public static void main(String[] args)
来源：http://ztq.andypj.xyz

Go:   func main()
来源：http://tuy.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fln.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://skj.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://izr.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://npl.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://twy.smart0.xyz

JS:   process.platform;  process.version
来源：http://exj.jyoumei.cn

TS:   process.platform;  process.version
来源：http://lmg.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rhv.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uad.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bpr.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://wft.iojbl.cn

================================================================================
来源：http://yqk.zhoulong.xyz

N. 数据结构与算法
来源：http://qso.aizwys.cn

================================================================================
来源：http://xso.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://jhn.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://cep.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xji.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ues.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ywc.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://czm.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://etg.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ack.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://fex.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://hul.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://knd.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fcu.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dxp.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://byc.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cdn.fengsongda.top

Go:   slices.Sort(arr)
来源：http://rth.nanxuanxn.top

Ruby: arr.sort
来源：http://tdl.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mpx.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://eqh.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qlp.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://fzg.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://njr.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://asg.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pho.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nzz.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zye.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://auj.fzhhl.top

[N04] 斐波那契数列
来源：http://elp.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ohv.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fks.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oup.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uqo.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tfj.hesvh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ufv.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wqw.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://chz.pengpengdd.cyou


<!-- 参考信息 -->