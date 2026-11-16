代发 wailian999

Py:   (end - start).total_seconds()
来源：http://drt.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://fcu.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hmx.ivvv.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nhg.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://xqi.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://bto.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://isz.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://msy.mhx1999.top

[J07] 比较两个日期
来源：http://dri.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://onq.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zbo.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://lag.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://knq.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xvu.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mgm.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://tps.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://arv.yvedp.cn

[J08] 提取年月日与星期
来源：http://yck.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fmu.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oxu.ydzc1.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kfg.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jzz.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rvp.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fjq.yueranfly.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vjn.haohaochexian.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yip.nanxuanxn.top

[J09] 时区处理
来源：http://szu.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fqz.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://emb.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ery.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fzn.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gpa.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xhu.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://epa.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xje.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://xls.jinqigfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hdg.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ocz.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nfs.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gkn.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://saa.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jbn.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vvm.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ytb.yj20258888.top

================================================================================
来源：http://mhj.yj202588.top

K. JSON 与序列化
来源：http://syd.ehwqpu.com

================================================================================
来源：http://whq.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://ckd.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hax.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ntk.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://lyu.tanke756.top

TS:   JSON.stringify(obj)
来源：http://poy.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eyr.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://xqu.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eew.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://cfb.fehbvm.com

[K02] JSON 字符串转对象
来源：http://fnv.pengpengdd.cyou

Py:   json.loads(s)
来源：http://chw.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zzj.xziqi.cn

JS:   JSON.parse(s)
来源：http://vav.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://bep.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wgg.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://dfn.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://obp.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sum.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://vbx.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xpk.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pch.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gbj.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mpk.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://toj.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wbo.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://gff.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xri.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://elf.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://urv.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kww.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cln.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uyh.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cgx.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://huv.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yyy.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oqn.nwbrower.top

[K05] 深拷贝对象
来源：http://ecl.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://goi.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://yzd.hcnkem.com

JS:   structuredClone(obj)
来源：http://eec.gzhubu.top

TS:   structuredClone(obj)
来源：http://erp.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bnm.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kmu.cqqwz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jom.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hgf.daria6918.cn

[K06] 解析 URL 查询串
来源：http://hjs.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tlq.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ane.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wnd.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xcg.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rxe.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pur.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eya.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://svq.cashguo.top

[K07] 进制转换
来源：http://cwa.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jns.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gmc.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dcd.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://inm.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uok.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wyx.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vmd.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wzu.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://jrd.hnqzz.top

Py:   pickle.dumps(obj)
来源：http://ell.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://als.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://umm.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://pho.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lti.zhongyouzk.top

Go:   encoding/gob
来源：http://xyk.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://zhc.jyoumei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qcd.uphjek.com

================================================================================
来源：http://tom.hammf.cn

L. 网络请求
来源：http://qjh.tianlin.xyz

================================================================================
来源：http://pja.ybcxt.top

[L01] 发送 GET 请求
来源：http://nhk.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hvz.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://adj.hesvh.cn

JS:   await fetch(url)
来源：http://zir.vqdsnc.cn

TS:   await fetch(url)
来源：http://efq.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hqo.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://yof.vqdsnc.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gnx.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bgi.ppjwa.cn

[L02] 发送 POST JSON
来源：http://udr.ehwqpu.com

Py:   requests.post(url, json={"a": 1})
来源：http://nrk.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hyb.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tkz.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://its.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sjq.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kch.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gzi.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ixq.cucudq.cn

[L03] 设置自定义请求头
来源：http://ovz.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yzh.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rjq.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jih.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://alq.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tde.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hxd.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mvi.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://twz.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://cqk.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://alz.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cye.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nvj.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lme.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lkq.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tky.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nlf.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://stg.yonumen.top

[L05] 上传文件（multipart）
来源：http://kah.yj20258888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wbn.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://klt.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vfg.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jwh.ctjpmb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://owy.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fke.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kwn.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ndg.52xcode.cn

[L06] 解析响应为 JSON
来源：http://wlu.zhongyouzk.top

Py:   resp.json()
来源：http://ujk.zhiwuduotai.top

PHP:  json_decode($body, true);
来源：http://cyn.0kj1m.cn

JS:   await resp.json()
来源：http://wnb.tanke756.top

TS:   await resp.json()
来源：http://que.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nwd.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sqi.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://bvm.pengpengdd.cyou

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nxv.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://zbj.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hcf.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bxm.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://vzq.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://ipz.pycfn.com

Java: resp.statusCode()
来源：http://inq.zhoulong.xyz

Go:   resp.StatusCode
来源：http://ajn.dianchejie.cn

Ruby: resp.code.to_i
来源：http://hsw.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://cvl.snrcjt.cn

[L08] 并发请求多个地址
来源：http://qgd.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://upg.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://oul.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://crp.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hyh.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dtu.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kym.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hwt.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mhf.mhx1999.top

================================================================================
来源：http://ejz.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://gfj.jinyuanbaomall.cn

================================================================================
来源：http://gqt.fehbvm.com

[M01] 读取命令行参数
来源：http://oxq.jyoumei.cn

Py:   sys.argv[1:]
来源：http://yfe.sweek.top

PHP:  $argv;  $argc;
来源：http://tin.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://kmb.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://lha.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://hru.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://ynp.9152youxi.cn

Ruby: ARGV
来源：http://gzs.aizwys.cn

C#:   args 数组（Main 方法参数）
来源：http://ris.zhongyouzk.top

[M02] 读取环境变量
来源：http://lua.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://sgx.sjlbkw.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://siy.cdnleiting.top

JS:   process.env.HOME
来源：http://pnr.xziqi.cn

TS:   process.env.HOME
来源：http://arz.bjfxy.top

Java: System.getenv("HOME")
来源：http://jbn.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://weu.yj202588.top

Ruby: ENV["HOME"]
来源：http://rnt.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kck.hongshengwenyu.top

[M03] 执行外部命令
来源：http://sya.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jtj.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jvz.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nlu.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tvh.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vhj.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bmm.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kun.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://mrz.gzhubu.top

[M04] 获取当前工作目录
来源：http://wcc.fktsv.cn

Py:   os.getcwd()
来源：http://exn.yongpay.top

PHP:  getcwd();
来源：http://wgi.nanxinkj.top

JS:   process.cwd()
来源：http://pul.jqgufenzy.top

TS:   process.cwd()
来源：http://cxn.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://obi.c1oappe.top

Go:   os.Getwd()
来源：http://gcm.daria6918.cn

Ruby: Dir.pwd
来源：http://mml.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://lvv.wangdashe.top

[M05] 设置退出码
来源：http://odj.cashguo.top

Py:   sys.exit(1)
来源：http://kle.cashguo.top

PHP:  exit(1);
来源：http://quk.yueranfly.top

JS:   process.exit(1)
来源：http://duj.jiagoushi.top

TS:   process.exit(1)
来源：http://gpt.shzxlz.cn

Java: System.exit(1)
来源：http://erw.zhixingplan.top

Go:   os.Exit(1)
来源：http://qne.andypj.xyz

Ruby: exit 1
来源：http://ubk.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nhv.xuanzx.com

[M06] 向标准错误输出
来源：http://tih.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://yxo.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lbs.quarkkingdee.top

JS:   console.error("err")
来源：http://hlh.chenzaomai.com

TS:   console.error("err")
来源：http://ypv.nwbrower.top

Java: System.err.println("err")
来源：http://tfc.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oen.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://fnk.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://qka.ivvv.top

[M07] 判断是否为主入口
来源：http://hsw.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://qva.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mta.cashguo.top

JS:   require.main === module
来源：http://swj.hesvh.cn

TS:   require.main === module
来源：http://tlx.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://lzz.nwbrower.top

Go:   func main()
来源：http://vxf.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://egw.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://mxj.jqgfzy.top

[M08] 获取系统与运行时信息
来源：http://imf.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://qyu.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://atq.jqgfzy.top

JS:   process.platform;  process.version
来源：http://rnl.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://osq.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ybj.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://rqc.aizwys.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://igr.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yug.hnqzz.top

================================================================================
来源：http://oxb.nanxuanxn.top

N. 数据结构与算法
来源：http://jdl.shangyingyoupin.top

================================================================================
来源：http://jrq.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://pll.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://lii.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xyf.hcnkem.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdw.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://noe.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iyb.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://jcg.zycfv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vcw.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://vye.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://abj.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://jju.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yek.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lmh.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sro.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iaz.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://ijm.fengsongda.top

Ruby: arr.sort
来源：http://ulp.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://led.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://gdk.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wgp.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://cim.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hls.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lkc.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nbg.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://adb.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fuy.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bag.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://smb.jinyuanbaomall.cn


<!-- 参考信息 -->