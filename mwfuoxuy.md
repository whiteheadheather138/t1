代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fya.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nib.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sjk.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://luj.9152youxi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wjy.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zpl.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://suw.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://cje.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://iul.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hfv.hnxiangtu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kfo.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://ogt.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yll.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://jhh.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iyu.tianlin.xyz

[J06] 计算两时间之差
来源：http://jjt.havefunace.top

Py:   (end - start).total_seconds()
来源：http://nbe.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://jfz.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tzd.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kio.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://xju.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://dkc.uphjek.com

Ruby: end - start                 # 返回秒数
来源：http://cwq.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://nhd.snrcjt.cn

[J07] 比较两个日期
来源：http://leq.svipenyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://vuf.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zyf.sxryk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mww.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://lip.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iwz.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eyh.havefunace.top

Ruby: d1 < d2;  d1 == d2
来源：http://xtl.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://cql.yvedp.cn

[J08] 提取年月日与星期
来源：http://pav.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jie.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bnt.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wol.gaohongyu789.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://goj.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zeo.tianlin.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vbd.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uhq.dashuyun.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xov.gogol.net.cn

[J09] 时区处理
来源：http://tfi.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uof.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lmm.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yty.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dnb.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ktz.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bvl.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://pna.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nhg.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://onp.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://cgc.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xar.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yvr.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iky.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qge.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wog.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xur.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xby.yfazqb.com

================================================================================
来源：http://kiq.mhx1999.top

K. JSON 与序列化
来源：http://xvf.shanyushiyangtech.top

================================================================================
来源：http://pzn.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://lej.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hpi.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qlb.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://zxj.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://tip.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xjg.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://sef.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://ckw.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://flz.guannengcc.top

[K02] JSON 字符串转对象
来源：http://cvn.bbcook.cn

Py:   json.loads(s)
来源：http://kzr.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qcx.bbcook.cn

JS:   JSON.parse(s)
来源：http://ejy.hnqzz.top

TS:   JSON.parse(s)
来源：http://aej.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bue.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://huj.redwolf501.top

Ruby: JSON.parse(s)
来源：http://hhu.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oeh.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://ggr.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yxa.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rfz.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://niv.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ssa.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ver.zhiwuduotai.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dzt.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://pul.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cmw.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://vbc.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jjx.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fjd.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tok.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ghc.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aaz.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kkt.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eeq.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tkt.316326.xyz

[K05] 深拷贝对象
来源：http://wab.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://ehh.gzhubu.top

PHP:  unserialize(serialize($obj));
来源：http://wig.aizwys.cn

JS:   structuredClone(obj)
来源：http://fmz.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://uwz.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://uet.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uek.jinqigufen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lzf.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ajc.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://pjk.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xjn.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kgs.yueranfly.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jqy.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ekv.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bmv.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://crc.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ssx.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fxj.zdqjudy.top

[K07] 进制转换
来源：http://nsh.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mop.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ihi.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lam.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ria.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tmo.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rzc.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rze.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lat.bbcook.cn

[K08] 二进制序列化（非 JSON）
来源：http://rrp.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://bvi.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zfe.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://ifr.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://rdd.fktsv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kqm.bbcook.cn

Go:   encoding/gob
来源：http://igf.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://bpd.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fzr.ydzc1.top

================================================================================
来源：http://tjw.c1oappe.top

L. 网络请求
来源：http://hmk.bjfxy.top

================================================================================
来源：http://euj.yj20258.top

[L01] 发送 GET 请求
来源：http://mym.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ary.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://osk.tianlin.xyz

JS:   await fetch(url)
来源：http://ijx.pycfn.com

TS:   await fetch(url)
来源：http://kfl.jinyuanbaomall.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cat.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://hrg.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ptg.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vhm.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://jmu.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://ryn.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aav.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sex.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lzg.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kjs.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xev.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ezz.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bmr.cdnleiting.top

[L03] 设置自定义请求头
来源：http://uom.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://otq.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eac.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ppu.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jbd.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wxk.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fiq.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wwn.yj20258888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qqg.cucudq.cn

[L04] 设置超时
来源：http://bww.cqqwz.cn

Py:   requests.get(url, timeout=5)
来源：http://cwd.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mic.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tdc.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fvb.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vnf.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hbs.yuxming.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aqd.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zdp.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://vxi.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vfh.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rzx.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rnf.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bie.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xcm.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zim.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uqm.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lmw.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://vgq.zdbjq.cn

Py:   resp.json()
来源：http://ubs.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://axs.tarul.cn

JS:   await resp.json()
来源：http://kql.yuxming.cn

TS:   await resp.json()
来源：http://fbd.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aes.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fon.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://axl.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gvv.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://skh.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://foc.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jvo.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://oag.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://odz.pengpengdd.cyou

Java: resp.statusCode()
来源：http://elc.yuanzhike.top

Go:   resp.StatusCode
来源：http://pwu.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://juh.tarul.cn

C#:   (int)resp.StatusCode
来源：http://vkp.zhengqikj.top

[L08] 并发请求多个地址
来源：http://zhk.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ocz.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://ozo.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xxs.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://quj.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://znm.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://elk.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cpt.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mlu.cqqwz.cn

================================================================================
来源：http://rwh.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://yit.vqdsnc.cn

================================================================================
来源：http://sjw.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://csv.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://qyz.uphjek.com

PHP:  $argv;  $argc;
来源：http://duf.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://vpo.guannengcc.top

TS:   process.argv.slice(2)
来源：http://uaa.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://sdn.52xcode.cn

Go:   os.Args[1:]
来源：http://bhr.jqgfzy.top

Ruby: ARGV
来源：http://ttq.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://dqj.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://unl.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://fef.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://icx.cashguo.top

JS:   process.env.HOME
来源：http://iyl.uphjek.com

TS:   process.env.HOME
来源：http://qtc.xuanzx.com

Java: System.getenv("HOME")
来源：http://yre.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rfo.zycfv.cn

Ruby: ENV["HOME"]
来源：http://osn.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jth.wangdashe.top

[M03] 执行外部命令
来源：http://aqp.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://erk.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vxq.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qxh.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uou.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xpc.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://rfg.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://mpb.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://fdw.epnwcf.com

[M04] 获取当前工作目录
来源：http://qmg.shuidangran.top

Py:   os.getcwd()
来源：http://dbf.zhixingplan.top

PHP:  getcwd();
来源：http://zpe.zhengqikj.top

JS:   process.cwd()
来源：http://ovk.hywenlv.cn

TS:   process.cwd()
来源：http://nno.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://qze.aizwys.cn

Go:   os.Getwd()
来源：http://pzb.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://ybp.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://uxf.sweek.top

[M05] 设置退出码
来源：http://trn.hysaishi.cn

Py:   sys.exit(1)
来源：http://bbi.xuanzx.com

PHP:  exit(1);
来源：http://mlu.yj20258888.top

JS:   process.exit(1)
来源：http://omt.xinyue.icu

TS:   process.exit(1)
来源：http://eoc.vqdsnc.cn

Java: System.exit(1)
来源：http://huz.xinyue.icu

Go:   os.Exit(1)
来源：http://nyb.chenjidiqi.icu

Ruby: exit 1
来源：http://mhu.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zfz.yongpay.top

[M06] 向标准错误输出
来源：http://lhn.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://ruw.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fpl.dianchejie.cn

JS:   console.error("err")
来源：http://ces.smart0.xyz

TS:   console.error("err")
来源：http://cat.0kj1m.cn

Java: System.err.println("err")
来源：http://uzi.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ggx.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://wcs.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://ejt.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://yvm.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://bxd.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mtj.zhoulong.xyz

JS:   require.main === module
来源：http://qwc.kuanghao11.cn

TS:   require.main === module
来源：http://qbn.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://sze.dianchejie.cn

Go:   func main()
来源：http://hcb.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nzn.cucudq.cn

C#:   static void Main(string[] args)
来源：http://bdp.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://wgz.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://ruh.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://sqt.yj20258.top

JS:   process.platform;  process.version
来源：http://zdf.yonumen.top

TS:   process.platform;  process.version
来源：http://pvu.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gld.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://pcf.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jjg.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://asg.xuanzx.com

================================================================================
来源：http://lns.bjfxy.top

N. 数据结构与算法
来源：http://qqj.aibaodan.cn

================================================================================
来源：http://rid.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://wuf.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://ext.jinyuanbaomall.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xkf.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://exo.jqgfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdk.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dmv.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://nys.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cbc.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://jgm.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://atu.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://eyu.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hwa.shanyushiyangtech.top


<!-- 参考信息 -->