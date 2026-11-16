代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://vhq.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://hwa.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://vti.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://ksk.sysykeji.top

[J07] 比较两个日期
来源：http://xan.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://fuo.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xzx.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://azn.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://kyv.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tjt.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://job.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rel.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://veo.cheryme.top

[J08] 提取年月日与星期
来源：http://hgg.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xpe.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bfh.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fta.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mcw.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qiz.jiagoushi.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://szc.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dog.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ddg.zhengqikj.top

[J09] 时区处理
来源：http://enp.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mkz.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cby.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ubm.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jrl.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dtt.yuxming.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sgz.uphjek.com

Ruby: Time.now.getlocal("+08:00")
来源：http://scc.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://igz.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://bmx.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://srz.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rii.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uxl.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ztu.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hrk.fktsv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yoz.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://grc.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bue.jyoumei.cn

================================================================================
来源：http://hbv.dashuyun.cn

K. JSON 与序列化
来源：http://djs.kuanghao11.cn

================================================================================
来源：http://owy.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://pja.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gyg.gotoacloud.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qsl.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://qbq.yonumen.top

TS:   JSON.stringify(obj)
来源：http://tsg.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wao.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://gvt.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://mfu.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fiz.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://qxk.yuanzhike.top

Py:   json.loads(s)
来源：http://nds.sweek.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vve.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://kfd.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://erm.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hbf.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://eea.xinyue.icu

Ruby: JSON.parse(s)
来源：http://rqf.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hxb.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://avc.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vtc.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yfb.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yyx.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yjh.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fsv.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qwq.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://jdb.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jwr.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://woz.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ttf.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nsc.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qhk.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cnc.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sdi.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ibo.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jya.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tnq.zdbjq.cn

[K05] 深拷贝对象
来源：http://jsu.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://lng.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://jag.zdqjudy.top

JS:   structuredClone(obj)
来源：http://ddz.sxryk.cn

TS:   structuredClone(obj)
来源：http://gtl.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://jnb.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rey.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dxt.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://lbr.shuidangran.top

[K06] 解析 URL 查询串
来源：http://grh.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qit.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sza.zycfv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tco.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mkn.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gso.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://twn.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cwz.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bke.daria6918.cn

[K07] 进制转换
来源：http://wxd.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://web.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lld.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vee.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lpm.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://euk.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://skf.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ies.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jbi.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://glr.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://vrx.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rvl.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://kqo.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://gty.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wvd.mhx1999.top

Go:   encoding/gob
来源：http://kic.hnxiangtu.top

Ruby: Marshal.dump(obj)
来源：http://xex.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://znv.smart0.xyz

================================================================================
来源：http://nul.zdqjudy.top

L. 网络请求
来源：http://ukz.svipenyu.cn

================================================================================
来源：http://ugz.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://ogk.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ukn.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://icy.tian-w.cn

JS:   await fetch(url)
来源：http://tzm.zhijiandao.cn

TS:   await fetch(url)
来源：http://ggx.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yug.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://mqy.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jxs.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oyu.hfpthk.cn

[L02] 发送 POST JSON
来源：http://sbd.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dux.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qri.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://utr.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tow.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ugs.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gdl.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fxh.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kry.gzhubu.top

[L03] 设置自定义请求头
来源：http://dkp.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wzt.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aji.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dfy.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kom.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sya.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://axh.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aqr.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ptx.birdmap.top

[L04] 设置超时
来源：http://ukq.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://uyu.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iyo.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fzn.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gpt.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fbq.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gtx.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lfj.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gtx.zycfv.cn

[L05] 上传文件（multipart）
来源：http://swf.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fmd.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wkf.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nog.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kze.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://igo.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://won.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jri.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dwl.cucudq.cn

[L06] 解析响应为 JSON
来源：http://ttg.hammf.cn

Py:   resp.json()
来源：http://kln.fzhhl.top

PHP:  json_decode($body, true);
来源：http://elu.jqgufenzy.top

JS:   await resp.json()
来源：http://lrg.hcnkem.com

TS:   await resp.json()
来源：http://nzm.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dpz.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cuo.hnxiangtu.top

Ruby: JSON.parse(resp.body)
来源：http://xor.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hqc.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://pbp.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wye.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wou.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://sgq.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://myt.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://vnc.sufxvd.cn

Go:   resp.StatusCode
来源：http://oce.yj20258.top

Ruby: resp.code.to_i
来源：http://yvh.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://wmi.xuanzx.com

[L08] 并发请求多个地址
来源：http://aeu.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hjd.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://yyw.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://orr.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://txl.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iuw.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://min.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fiy.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gqe.yonumen.top

================================================================================
来源：http://zkz.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://jin.snrcjt.cn

================================================================================
来源：http://ylx.tian-w.cn

[M01] 读取命令行参数
来源：http://rtq.xylfe.cn

Py:   sys.argv[1:]
来源：http://lot.52xcode.cn

PHP:  $argv;  $argc;
来源：http://ryt.birdmap.top

JS:   process.argv.slice(2)
来源：http://gyn.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://grg.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://ash.ehwqpu.com

Go:   os.Args[1:]
来源：http://jzy.yanxiufei.cn

Ruby: ARGV
来源：http://jmy.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://jos.haohaochexian.top

[M02] 读取环境变量
来源：http://hqm.yonumen.top

Py:   os.environ.get("HOME")
来源：http://ryx.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xrv.tanke756.top

JS:   process.env.HOME
来源：http://kpn.zhixingplan.top

TS:   process.env.HOME
来源：http://ntc.yangfankeji.com

Java: System.getenv("HOME")
来源：http://dsw.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://feb.hnqzz.top

Ruby: ENV["HOME"]
来源：http://qkt.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bym.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://mxy.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dcg.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jzt.hnqzz.top

JS:   child_process.execSync("ls -l").toString()
来源：http://uqo.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lav.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rvd.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lfc.sufxvd.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yfq.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://dnr.haohaochexian.top

[M04] 获取当前工作目录
来源：http://bcb.hesvh.cn

Py:   os.getcwd()
来源：http://fuj.9152youxi.cn

PHP:  getcwd();
来源：http://lyb.yj20258888.top

JS:   process.cwd()
来源：http://bmh.sysykeji.top

TS:   process.cwd()
来源：http://xyn.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://hrl.hnqzz.top

Go:   os.Getwd()
来源：http://sry.sufxvd.cn

Ruby: Dir.pwd
来源：http://qjd.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://nwo.jyoumei.cn

[M05] 设置退出码
来源：http://eno.chenzaomai.com

Py:   sys.exit(1)
来源：http://gcp.sweek.top

PHP:  exit(1);
来源：http://ezu.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://ybr.cucudq.cn

TS:   process.exit(1)
来源：http://hlf.fktsv.cn

Java: System.exit(1)
来源：http://wwn.yanxiufei.cn

Go:   os.Exit(1)
来源：http://qre.pycfn.com

Ruby: exit 1
来源：http://mcx.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ykh.havefunace.top

[M06] 向标准错误输出
来源：http://cax.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://cmd.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wwq.aizwys.cn

JS:   console.error("err")
来源：http://jjl.andypj.xyz

TS:   console.error("err")
来源：http://cel.zycfv.cn

Java: System.err.println("err")
来源：http://jfu.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wsb.ydjk.org.cn

Ruby: warn "err"
来源：http://mxs.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://nzh.jianghu66.top

[M07] 判断是否为主入口
来源：http://gvn.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://boe.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fzl.hongshengwenyu.top

JS:   require.main === module
来源：http://gcv.guannengcc.top

TS:   require.main === module
来源：http://tqn.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://wiy.zhongyouzk.top

Go:   func main()
来源：http://bhb.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://knl.yj20258.top

C#:   static void Main(string[] args)
来源：http://tau.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://wrd.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://wgh.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://rgg.cashguo.top

JS:   process.platform;  process.version
来源：http://vir.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://uhk.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zib.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bes.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://opn.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uox.vqdsnc.cn

================================================================================
来源：http://fvu.fehbvm.com

N. 数据结构与算法
来源：http://xbo.tarul.cn

================================================================================
来源：http://fzc.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://fqr.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://znm.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://phy.hcnkem.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yaz.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oef.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://nkg.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://jgz.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://uyk.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xzb.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://evy.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://sbt.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gct.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yon.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://srm.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://flf.hnqzz.top

Go:   slices.Sort(arr)
来源：http://mdh.zhoulong.xyz

Ruby: arr.sort
来源：http://feb.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ffu.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://ija.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iij.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://wvt.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rph.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gsm.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xih.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lms.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jpd.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://jok.fzhhl.top

[N04] 斐波那契数列
来源：http://smy.jqgufenzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jmv.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jqv.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qrb.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ick.zhoulong.xyz


<!-- 参考信息 -->