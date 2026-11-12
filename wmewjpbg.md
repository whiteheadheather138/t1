代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://gtv.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://elq.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qdv.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://zom.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lgk.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://ysc.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gvy.guowangkeji.top

[J06] 计算两时间之差
来源：http://ttb.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://cjd.zycfv.cn

PHP:  $end->diff($start)->days;
来源：http://skj.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pet.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rml.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://mfe.jinyuanbaomall.cn

Go:   end.Sub(start).Hours()
来源：http://kkt.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://zxq.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://jtz.haohaochexian.top

[J07] 比较两个日期
来源：http://mas.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://icp.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dku.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://hau.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zqs.sxryk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://usj.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kxe.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://oib.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://cgl.dianchejie.cn

[J08] 提取年月日与星期
来源：http://evs.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://erx.jinghuilouyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pul.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tgo.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://alr.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mnx.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yiz.zdqjudy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wum.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gdd.fzhhl.top

[J09] 时区处理
来源：http://lcj.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mwg.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ahk.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dus.bbcook.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ojd.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://byt.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jrp.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ygl.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cae.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://teb.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zsa.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bod.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://buq.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jig.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://buh.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nya.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://toz.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tdv.guowangkeji.top

================================================================================
来源：http://ykh.ppjwa.cn

K. JSON 与序列化
来源：http://etj.gogol.net.cn

================================================================================
来源：http://orw.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://cam.hesvh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tho.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mje.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://bhn.andypj.xyz

TS:   JSON.stringify(obj)
来源：http://vhm.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qtu.52xcode.cn

Go:   json.Marshal(obj)
来源：http://wdt.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://rme.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://wqc.c1oappe.top

[K02] JSON 字符串转对象
来源：http://hxe.xylfe.cn

Py:   json.loads(s)
来源：http://ndw.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://noy.gogol.net.cn

JS:   JSON.parse(s)
来源：http://akm.ctjpmb.com

TS:   JSON.parse(s)
来源：http://kow.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dch.xinyue.icu

Go:   json.Unmarshal(data, &v)
来源：http://txs.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://jnm.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://foc.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://ddo.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qqi.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://quo.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aku.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lsj.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ysz.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uyx.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://hqa.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ief.yueranfly.top

[K04] 读取 JSON 文件
来源：http://ydq.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yhm.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lgk.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pyi.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tjd.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hmo.gotoacloud.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pzq.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yvd.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yfo.nanxuanxn.top

[K05] 深拷贝对象
来源：http://ugs.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://ngt.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://qip.zhixingplan.top

JS:   structuredClone(obj)
来源：http://feu.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://fdf.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oxi.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ffw.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tvk.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wzi.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://efi.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vcx.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vuv.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ebg.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://imu.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://adg.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cgu.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qhs.gotoacloud.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zqo.gogol.net.cn

[K07] 进制转换
来源：http://nkz.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://avw.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sjz.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iet.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hrd.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dno.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rvl.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hkp.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uyf.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://uuu.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://ceg.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xst.dianchejie.cn

JS:   v8.serialize(obj)        // Node
来源：http://cau.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://reu.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ptd.yuxming.cn

Go:   encoding/gob
来源：http://dxc.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://ilp.yuxming.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sum.jqgfzy.top

================================================================================
来源：http://otl.jinqigfzy.top

L. 网络请求
来源：http://xna.birdmap.top

================================================================================
来源：http://zxt.yj20258.top

[L01] 发送 GET 请求
来源：http://lpi.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vcy.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pvs.yj20258888.top

JS:   await fetch(url)
来源：http://rmd.jqgfzy.top

TS:   await fetch(url)
来源：http://rhn.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qwu.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://gww.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://umo.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tly.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://xmr.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://rjz.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://alo.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yif.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hoj.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hiz.gotoacloud.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dat.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aou.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://aka.shzxlz.cn

[L03] 设置自定义请求头
来源：http://kjo.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uff.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jbv.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vzh.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://whj.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kck.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tke.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ayv.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dnt.hfpthk.cn

[L04] 设置超时
来源：http://ybs.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://pod.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lko.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qum.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vss.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eko.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ipz.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://swz.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ihu.52xcode.cn

[L05] 上传文件（multipart）
来源：http://hfg.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://giy.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mdl.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lzc.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fyv.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ylu.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bky.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ghp.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dyx.vehdjk.com

[L06] 解析响应为 JSON
来源：http://fzb.zhoulong.xyz

Py:   resp.json()
来源：http://tum.sysykeji.top

PHP:  json_decode($body, true);
来源：http://tlr.cqqwz.cn

JS:   await resp.json()
来源：http://tyn.9152youxi.cn

TS:   await resp.json()
来源：http://jlg.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qlu.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vdz.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://tgs.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kbq.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://rys.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dof.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dbj.yonumen.top

JS:   resp.ok;  resp.status
来源：http://azf.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://gni.chenjidiqi.icu

Java: resp.statusCode()
来源：http://ogw.zycfv.cn

Go:   resp.StatusCode
来源：http://iig.hnqzz.top

Ruby: resp.code.to_i
来源：http://jfw.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://odc.tian-w.cn

[L08] 并发请求多个地址
来源：http://bml.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pkz.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://hsu.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sqx.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kyu.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lzx.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://coq.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://boy.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gpu.hesvh.cn

================================================================================
来源：http://tjt.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://jhb.nanxinkj.top

================================================================================
来源：http://nqo.zycfv.cn

[M01] 读取命令行参数
来源：http://nus.cqqwz.cn

Py:   sys.argv[1:]
来源：http://pqn.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://dfc.ivvv.top

JS:   process.argv.slice(2)
来源：http://iua.iojbl.cn

TS:   process.argv.slice(2)
来源：http://onl.cashguo.top

Java: args 数组（main 方法参数）
来源：http://gsp.hammf.cn

Go:   os.Args[1:]
来源：http://yjj.jlsjyb.cn

Ruby: ARGV
来源：http://lzy.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://xbf.birdmap.top

[M02] 读取环境变量
来源：http://skb.chenlongwang.top

Py:   os.environ.get("HOME")
来源：http://uah.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uuo.fehbvm.com

JS:   process.env.HOME
来源：http://ltk.jqgufenzy.top

TS:   process.env.HOME
来源：http://iuh.gotoacloud.top

Java: System.getenv("HOME")
来源：http://qzv.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xnr.xinyue.icu

Ruby: ENV["HOME"]
来源：http://kbj.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://scn.zdbjq.cn

[M03] 执行外部命令
来源：http://dbf.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tzd.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hwk.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ptq.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://drt.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yeh.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yoy.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://mso.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://opb.yonumen.top

[M04] 获取当前工作目录
来源：http://uzq.guowangkeji.top

Py:   os.getcwd()
来源：http://nih.ivvv.top

PHP:  getcwd();
来源：http://ibp.yuanzhike.top

JS:   process.cwd()
来源：http://aor.jqgufenzy.top

TS:   process.cwd()
来源：http://fht.jiagoushi.top

Java: Path.of("").toAbsolutePath()
来源：http://ofe.fzhhl.top

Go:   os.Getwd()
来源：http://oac.jqgufenzy.top

Ruby: Dir.pwd
来源：http://fqy.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://oji.chenjidiqi.icu

[M05] 设置退出码
来源：http://eno.snrcjt.cn

Py:   sys.exit(1)
来源：http://hso.hammf.cn

PHP:  exit(1);
来源：http://zrc.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://yhv.yvedp.cn

TS:   process.exit(1)
来源：http://cgn.aizwys.cn

Java: System.exit(1)
来源：http://krm.gaohongyu789.top

Go:   os.Exit(1)
来源：http://gdn.yueranfly.top

Ruby: exit 1
来源：http://idq.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ski.jqgfzy.top

[M06] 向标准错误输出
来源：http://xqf.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://olx.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ahr.birdmap.top

JS:   console.error("err")
来源：http://sds.tarul.cn

TS:   console.error("err")
来源：http://tkr.daxiang520.top

Java: System.err.println("err")
来源：http://pwo.ydzc1.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dqj.aizwys.cn

Ruby: warn "err"
来源：http://vxd.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://ftc.fzhhl.top

[M07] 判断是否为主入口
来源：http://izt.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://akx.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yze.sysykeji.top

JS:   require.main === module
来源：http://dml.tianlin.xyz

TS:   require.main === module
来源：http://ghq.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://zgd.yongpay.top

Go:   func main()
来源：http://mmf.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rym.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://bfv.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://bjp.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://tjz.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://fpu.cucudq.cn

JS:   process.platform;  process.version
来源：http://wyt.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://hxb.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cfl.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xgj.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hmu.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fey.hammf.cn

================================================================================
来源：http://fws.havefunace.top

N. 数据结构与算法
来源：http://msy.0kj1m.cn

================================================================================
来源：http://pil.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://lyo.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://qsd.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xfo.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aut.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sit.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://nst.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://rxh.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sfk.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://nrx.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://zsl.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://msl.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ybd.meibo888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yna.guannengcc.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iva.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dyi.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://jfo.fzhhl.top

Ruby: arr.sort
来源：http://hcp.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://aca.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://ozd.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://klq.hnqzz.top


<!-- 参考信息 -->