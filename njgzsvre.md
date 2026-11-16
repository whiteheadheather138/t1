代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://ivm.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://ydy.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://rlm.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://mdi.tanke756.top

[J07] 比较两个日期
来源：http://wkh.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://jbh.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wbr.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://ety.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://dks.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://plb.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://san.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://jnh.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://soq.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://weq.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ktu.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gyl.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kyr.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jkn.tian-w.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ryb.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mev.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pec.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ufd.jinqigufen.top

[J09] 时区处理
来源：http://kar.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qqq.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zcu.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wsi.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzn.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gfd.hysaishi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qqq.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ebh.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lte.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://vuc.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lji.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vyp.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uiy.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://puw.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://odx.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://djk.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tld.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ogb.jinqigfzy.top

================================================================================
来源：http://kxm.aibaodan.cn

K. JSON 与序列化
来源：http://uyw.jqgfzy.top

================================================================================
来源：http://vmd.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://djb.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wfn.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oxg.pycfn.com

JS:   JSON.stringify(obj)
来源：http://umk.tanke756.top

TS:   JSON.stringify(obj)
来源：http://ndy.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fsy.c1oappe.top

Go:   json.Marshal(obj)
来源：http://xxm.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://jbk.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tku.birdmap.top

[K02] JSON 字符串转对象
来源：http://fug.jinqigufen.top

Py:   json.loads(s)
来源：http://dti.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gaq.bjfxy.top

JS:   JSON.parse(s)
来源：http://bes.snrcjt.cn

TS:   JSON.parse(s)
来源：http://aqh.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uqy.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://tto.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://htg.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bzn.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://hcl.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dcu.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bil.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qbl.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://txy.vqdsnc.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yka.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mhn.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://kvs.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kfx.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://grj.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ydu.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tog.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aua.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mba.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aqe.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vkm.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://let.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vgt.redwolf501.top

[K05] 深拷贝对象
来源：http://kxn.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://xcf.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://crp.chenzaomai.com

JS:   structuredClone(obj)
来源：http://owr.aibaodan.cn

TS:   structuredClone(obj)
来源：http://tuu.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ope.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fbf.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://adv.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cmp.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://kqj.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ugx.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gjz.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gtr.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tra.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rmc.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qfj.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xkq.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yht.hfpthk.cn

[K07] 进制转换
来源：http://lxo.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nek.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oxs.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kmi.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gmx.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://twy.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nwb.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mwe.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wtx.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://wwx.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://xny.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lbi.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://zgf.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://bxc.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fdj.hnqzz.top

Go:   encoding/gob
来源：http://snn.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://rnw.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qsv.cucudq.cn

================================================================================
来源：http://crt.zhengqikj.top

L. 网络请求
来源：http://fpu.epnwcf.com

================================================================================
来源：http://flc.sweek.top

[L01] 发送 GET 请求
来源：http://axs.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xaj.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zyn.snrcjt.cn

JS:   await fetch(url)
来源：http://vyy.ydzc1.top

TS:   await fetch(url)
来源：http://xnc.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hls.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://whv.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vwo.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tgu.yonumen.top

[L02] 发送 POST JSON
来源：http://brq.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bxb.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ngd.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vus.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iuw.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zra.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lsn.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hka.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://naz.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://ttr.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://win.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lrp.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tpy.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wny.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dwr.andypj.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ypn.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fhl.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pjw.jqgufenzy.top

[L04] 设置超时
来源：http://sid.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://nsk.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://glu.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tci.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qkp.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zhd.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://put.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fzv.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kcp.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://xhp.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://swd.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fcw.hnxiangtu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tiw.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vji.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://llz.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mme.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bsd.yj202588.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fbm.tianlin.xyz

[L06] 解析响应为 JSON
来源：http://bwl.bbcook.cn

Py:   resp.json()
来源：http://fnt.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://onz.zhengqikj.top

JS:   await resp.json()
来源：http://bns.nanxuanxn.top

TS:   await resp.json()
来源：http://pvj.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tfl.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vgo.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://pro.ehwqpu.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yuv.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://yhw.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rod.jianghu66.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cll.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://uql.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://dsx.shangyingyoupin.top

Java: resp.statusCode()
来源：http://bhx.yj20258888.top

Go:   resp.StatusCode
来源：http://mau.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://guq.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://dwp.gogol.net.cn

[L08] 并发请求多个地址
来源：http://vrd.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jcg.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://ocd.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hgb.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blv.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ber.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://liz.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://end.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jki.wangshuangyany.cn

================================================================================
来源：http://mal.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://igc.gotoacloud.top

================================================================================
来源：http://yax.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://dbi.yueranfly.top

Py:   sys.argv[1:]
来源：http://jcx.cashguo.top

PHP:  $argv;  $argc;
来源：http://akj.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://tgc.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://igh.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://oqg.ppjwa.cn

Go:   os.Args[1:]
来源：http://xav.yuanzhike.top

Ruby: ARGV
来源：http://uoc.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://bjz.fzhhl.top

[M02] 读取环境变量
来源：http://xbs.gaohongyu789.top

Py:   os.environ.get("HOME")
来源：http://mle.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vuk.meibo888.top

JS:   process.env.HOME
来源：http://zll.wangdashe.top

TS:   process.env.HOME
来源：http://yyk.fktsv.cn

Java: System.getenv("HOME")
来源：http://onu.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kpw.316326.xyz

Ruby: ENV["HOME"]
来源：http://acj.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hwy.jinqigufen.top

[M03] 执行外部命令
来源：http://ngk.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tag.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lyi.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kfi.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://czi.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zsg.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://elj.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://eqc.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://mia.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://rqa.yj20258888.top

Py:   os.getcwd()
来源：http://jmn.fehbvm.com

PHP:  getcwd();
来源：http://can.xylfe.cn

JS:   process.cwd()
来源：http://nck.yuxming.cn

TS:   process.cwd()
来源：http://vup.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://oxp.feifeiyinyue.top

Go:   os.Getwd()
来源：http://vdw.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://vrh.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jmy.daria6918.cn

[M05] 设置退出码
来源：http://ygo.ybcxt.top

Py:   sys.exit(1)
来源：http://ety.xuetiantiany.cn

PHP:  exit(1);
来源：http://jzo.quarkkingdee.top

JS:   process.exit(1)
来源：http://nnh.hongshengwenyu.top

TS:   process.exit(1)
来源：http://qjf.tian-w.cn

Java: System.exit(1)
来源：http://izz.hesvh.cn

Go:   os.Exit(1)
来源：http://dyy.shanyushiyangtech.top

Ruby: exit 1
来源：http://uyd.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://afm.uphjek.com

[M06] 向标准错误输出
来源：http://tbb.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://krt.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ikh.nanxuanxn.top

JS:   console.error("err")
来源：http://hdg.andypj.xyz

TS:   console.error("err")
来源：http://wvb.yongpay.top

Java: System.err.println("err")
来源：http://zvn.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qgv.zhiwuduotai.top

Ruby: warn "err"
来源：http://oio.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://lrw.bbcook.cn

[M07] 判断是否为主入口
来源：http://rdf.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://zai.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kgv.shanyushiyangtech.top

JS:   require.main === module
来源：http://zke.gaohongyu789.top

TS:   require.main === module
来源：http://qnt.tian-w.cn

Java: public static void main(String[] args)
来源：http://dci.shuidangran.top

Go:   func main()
来源：http://abn.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gur.wangdashe.top

C#:   static void Main(string[] args)
来源：http://umi.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://ilx.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://odb.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://ubx.chenzaomai.com

JS:   process.platform;  process.version
来源：http://ohc.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://ctg.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iuf.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gab.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://axw.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ajy.jqgufenzy.top

================================================================================
来源：http://qao.chenjidiqi.icu

N. 数据结构与算法
来源：http://twb.yvedp.cn

================================================================================
来源：http://hcm.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://fnz.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vbd.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qjm.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zkw.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wtn.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://swt.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://hcn.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dwb.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://rod.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://bxu.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://lnw.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fgz.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oae.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://lmv.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rut.gaohongyu789.top

Go:   slices.Sort(arr)
来源：http://wjj.daxiang520.top

Ruby: arr.sort
来源：http://zib.daria6918.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zln.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://esg.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oxa.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://bdj.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jlv.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://don.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://axx.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uxj.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mhl.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://qgg.yangfankeji.com

[N04] 斐波那契数列
来源：http://hec.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uhf.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nlz.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://asf.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eul.zhijiandao.cn


<!-- 参考信息 -->