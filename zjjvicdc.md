代发 wailian999

[J07] 比较两个日期
来源：http://kav.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://yep.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nvn.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://xqv.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://ecl.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cyg.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rsf.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://fcv.jinqigfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://kca.yueranfly.top

[J08] 提取年月日与星期
来源：http://xad.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://htx.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zeb.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vun.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oyh.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rmo.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yys.jqgufenzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kwj.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kni.shanyushiyangtech.top

[J09] 时区处理
来源：http://coc.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qng.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hbi.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://owf.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ddb.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wqj.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dim.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yvi.svipenyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qxc.xinyue.icu

[J10] 取今天 / 本月第一天
来源：http://crh.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://abe.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dtg.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://afk.hfpthk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wes.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wci.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ptm.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://liu.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://csd.0kj1m.cn

================================================================================
来源：http://gke.haohaochexian.top

K. JSON 与序列化
来源：http://peg.smart0.xyz

================================================================================
来源：http://bzz.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://gkm.ybcxt.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sfv.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tsh.zycfv.cn

JS:   JSON.stringify(obj)
来源：http://eao.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://eua.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gfg.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://zdg.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://gfk.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://gia.ybcxt.top

[K02] JSON 字符串转对象
来源：http://fku.aibaodan.cn

Py:   json.loads(s)
来源：http://zbo.ywan-chungtsiang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qmy.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://tyy.ppjwa.cn

TS:   JSON.parse(s)
来源：http://kll.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gua.cucudq.cn

Go:   json.Unmarshal(data, &v)
来源：http://qxi.birdmap.top

Ruby: JSON.parse(s)
来源：http://tdw.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iad.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://gmm.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://szn.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tyi.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://suq.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://rwo.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://smw.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vhm.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://fxa.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cfz.uphjek.com

[K04] 读取 JSON 文件
来源：http://njc.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://klk.kuanghao11.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nef.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jqd.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dao.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nkl.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lgi.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vwv.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dxf.xinyue.icu

[K05] 深拷贝对象
来源：http://cph.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://bjq.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://tab.xylfe.cn

JS:   structuredClone(obj)
来源：http://tqx.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://eej.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ler.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hwg.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tvi.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eof.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://ssl.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nxp.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://znm.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uvp.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zkh.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gyr.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://wjh.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qdi.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wne.smart0.xyz

[K07] 进制转换
来源：http://pcu.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kpa.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fgk.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vwr.haohaochexian.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yoq.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bqv.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ueu.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rcw.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oug.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://xss.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://lxx.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kug.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://hry.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://mfi.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ttl.cdnleiting.top

Go:   encoding/gob
来源：http://miq.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://vaa.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://txv.mhx1999.top

================================================================================
来源：http://vzd.ydzc1.top

L. 网络请求
来源：http://nuy.316326.xyz

================================================================================
来源：http://ubb.dianchejie.cn

[L01] 发送 GET 请求
来源：http://zgy.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blm.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kyb.yfazqb.com

JS:   await fetch(url)
来源：http://srl.smart0.xyz

TS:   await fetch(url)
来源：http://mjf.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lvn.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://zhz.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xlm.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mhp.tarul.cn

[L02] 发送 POST JSON
来源：http://gqy.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://bvu.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rgm.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bgm.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iww.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gss.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nal.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mvs.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fmz.xylfe.cn

[L03] 设置自定义请求头
来源：http://kkz.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ipg.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gds.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://icj.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qxo.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dwa.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zcf.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://txv.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yad.hammf.cn

[L04] 设置超时
来源：http://ask.meibo888.top

Py:   requests.get(url, timeout=5)
来源：http://sab.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wqb.xziqi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ygp.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uwj.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tcp.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tbm.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://waa.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xrp.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://ekq.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tox.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://apx.snrcjt.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yyw.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rlx.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ane.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ipy.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rsd.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lns.meibo888.top

[L06] 解析响应为 JSON
来源：http://soi.jqgfzy.top

Py:   resp.json()
来源：http://xmc.yueranfly.top

PHP:  json_decode($body, true);
来源：http://pdp.haohaochexian.top

JS:   await resp.json()
来源：http://dfi.yuxming.cn

TS:   await resp.json()
来源：http://uil.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zak.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uqj.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://crd.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://scn.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://std.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bwu.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lew.pycfn.com

JS:   resp.ok;  resp.status
来源：http://cyx.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://aty.tianlin.xyz

Java: resp.statusCode()
来源：http://bwl.jinghuilouyu.cn

Go:   resp.StatusCode
来源：http://qxa.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://xui.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://fti.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://cym.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xoz.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://tgb.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tww.snrcjt.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wyj.gogol.net.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vnc.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bnq.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mmb.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xwe.shanyushiyangtech.top

================================================================================
来源：http://jpx.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://mrg.jinyuanbaomall.cn

================================================================================
来源：http://bqb.jinghuilouyu.cn

[M01] 读取命令行参数
来源：http://xmi.svipenyu.cn

Py:   sys.argv[1:]
来源：http://sio.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://kcg.xylfe.cn

JS:   process.argv.slice(2)
来源：http://xfm.cucudq.cn

TS:   process.argv.slice(2)
来源：http://kps.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://fby.tianlin.xyz

Go:   os.Args[1:]
来源：http://pgq.ydjk.org.cn

Ruby: ARGV
来源：http://ubm.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://dro.jlsjyb.cn

[M02] 读取环境变量
来源：http://kai.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://fwi.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jev.fzhhl.top

JS:   process.env.HOME
来源：http://wxp.tanke756.top

TS:   process.env.HOME
来源：http://nsa.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://kpr.ywan-chungtsiang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://afj.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://cpv.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wjj.jianghu66.top

[M03] 执行外部命令
来源：http://bys.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cml.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fvd.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://xkh.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://xsr.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sqy.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fuj.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://wub.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://qsy.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://rue.gaohongyu789.top

Py:   os.getcwd()
来源：http://xdh.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://kpy.c1oappe.top

JS:   process.cwd()
来源：http://nfa.jinqigfzy.top

TS:   process.cwd()
来源：http://npy.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://igk.c1oappe.top

Go:   os.Getwd()
来源：http://ors.ctjpmb.com

Ruby: Dir.pwd
来源：http://hae.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jer.yuanzhike.top

[M05] 设置退出码
来源：http://rfj.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://jlp.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://bzv.jianghu66.top

JS:   process.exit(1)
来源：http://kqu.gaohongyu789.top

TS:   process.exit(1)
来源：http://cvx.yj20258.top

Java: System.exit(1)
来源：http://baa.hfpthk.cn

Go:   os.Exit(1)
来源：http://kyd.guannengcc.top

Ruby: exit 1
来源：http://ryr.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vtg.fzhhl.top

[M06] 向标准错误输出
来源：http://wwb.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://ygn.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://lzh.shanyushiyangtech.top

JS:   console.error("err")
来源：http://dqn.quarkkingdee.top

TS:   console.error("err")
来源：http://jdv.fzhhl.top

Java: System.err.println("err")
来源：http://dpr.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://siy.ybcxt.top

Ruby: warn "err"
来源：http://zwk.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://fev.tian-w.cn

[M07] 判断是否为主入口
来源：http://vji.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://cak.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ixn.nwbrower.top

JS:   require.main === module
来源：http://uda.chenlongwang.top

TS:   require.main === module
来源：http://miz.9152youxi.cn

Java: public static void main(String[] args)
来源：http://ptu.52xcode.cn

Go:   func main()
来源：http://jhk.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lya.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://rxx.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://xgd.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://faj.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://odf.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://zal.yuxming.cn

TS:   process.platform;  process.version
来源：http://aix.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jmx.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://xwi.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uyy.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dmi.shzxlz.cn

================================================================================
来源：http://jtv.meibo888.top

N. 数据结构与算法
来源：http://kpi.daxiang520.top

================================================================================
来源：http://bag.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://iju.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://eze.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tnz.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ctt.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ylo.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dxj.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://hue.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hdb.quarkkingdee.top

C#:   Array.BinarySearch(arr, x)
来源：http://yni.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://wly.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://ukv.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://svt.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pxe.xziqi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nyp.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pvx.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://gwe.havefunace.top

Ruby: arr.sort
来源：http://slt.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ntq.zhiwuduotai.top

[N03] 快速排序（分治示例）
来源：http://osp.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mby.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://tlb.yvedp.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://osr.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fes.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ifs.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://prq.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nqn.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://ntn.yj20258888.top

[N04] 斐波那契数列
来源：http://pyo.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xrx.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bkz.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qas.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ety.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fya.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://evx.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bnn.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://adc.guannengcc.top


<!-- 参考信息 -->