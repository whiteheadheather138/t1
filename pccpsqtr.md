代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://grt.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://tjn.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://thl.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://lvt.yj20258.top

[J07] 比较两个日期
来源：http://zub.cdnleiting.top

Py:   d1 < d2;  d1 == d2
来源：http://sph.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zfz.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://cem.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://guo.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ird.zycfv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tje.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://qop.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://wxo.yongpay.top

[J08] 提取年月日与星期
来源：http://zub.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lwp.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iqv.yj20258888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cdu.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://deb.xinyue.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cpm.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lot.haohaochexian.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fup.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cuj.sxryk.cn

[J09] 时区处理
来源：http://jxh.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zcz.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yqg.zycfv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dwi.xziqi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jjw.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nzw.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://stz.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sqn.cdnleiting.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vae.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://qfg.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tsl.ydjk.org.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lcw.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bki.zycfv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ely.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jpd.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ovb.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://osw.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://slr.yvedp.cn

================================================================================
来源：http://aaq.hfpthk.cn

K. JSON 与序列化
来源：http://rqy.shangyingyoupin.top

================================================================================
来源：http://qxg.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://sdw.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fki.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ahz.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://mjo.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://sas.zdqjudy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ysz.52xcode.cn

Go:   json.Marshal(obj)
来源：http://xlp.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://inr.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uvx.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://htp.zhengqikj.top

Py:   json.loads(s)
来源：http://wom.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vrv.xinyue.icu

JS:   JSON.parse(s)
来源：http://xte.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://azm.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cok.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://lgf.ydzc1.top

Ruby: JSON.parse(s)
来源：http://jdq.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qiy.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://vbw.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kwe.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yej.hnxiangtu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xvl.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://swm.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tbm.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://okw.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://icf.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qxj.tanke756.top

[K04] 读取 JSON 文件
来源：http://tky.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aow.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ipy.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jbb.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uaj.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nzg.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zwi.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://frh.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kkh.jinqigufen.top

[K05] 深拷贝对象
来源：http://emy.aizwys.cn

Py:   copy.deepcopy(obj)
来源：http://omv.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://pud.iojbl.cn

JS:   structuredClone(obj)
来源：http://bun.hfpthk.cn

TS:   structuredClone(obj)
来源：http://dcv.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pwl.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fxf.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ycf.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://feh.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://krl.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fmo.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kiw.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pju.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bfv.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ccq.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lid.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rck.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ovk.xinyue.icu

[K07] 进制转换
来源：http://vqi.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qcy.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://afp.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aau.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wjm.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ehg.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://srr.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qfp.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pvf.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://opn.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://wzu.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://txj.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://amh.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://drd.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fbm.jianghu66.top

Go:   encoding/gob
来源：http://ldm.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://qod.redwolf501.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hgz.jqgfzy.top

================================================================================
来源：http://fvb.hnqzz.top

L. 网络请求
来源：http://lod.fanxiaobao.xyz

================================================================================
来源：http://yjv.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://djy.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xbz.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eud.52xcode.cn

JS:   await fetch(url)
来源：http://opw.ctjpmb.com

TS:   await fetch(url)
来源：http://jgu.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dos.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://pvp.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dxr.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kot.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://ybn.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://bfv.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hja.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hga.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bnd.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jvl.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kyj.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yew.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qsp.zhengqikj.top

[L03] 设置自定义请求头
来源：http://ahr.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oty.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://equ.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pik.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gkb.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nfm.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hup.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yuh.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qwa.epnwcf.com

[L04] 设置超时
来源：http://lsg.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://rmo.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uby.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oic.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uwe.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kub.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gmh.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lpv.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mdl.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://sug.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bjw.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qik.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nlq.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ecs.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uil.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hzm.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tcl.fengsongda.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pdq.shuidangran.top

[L06] 解析响应为 JSON
来源：http://cio.sysykeji.top

Py:   resp.json()
来源：http://kst.guannengcc.top

PHP:  json_decode($body, true);
来源：http://zcr.vqdsnc.cn

JS:   await resp.json()
来源：http://pgw.yanxiufei.cn

TS:   await resp.json()
来源：http://jzb.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dxg.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vuu.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://ggm.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ofb.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://jch.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://opc.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://atd.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://pym.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://qit.hcnkem.com

Java: resp.statusCode()
来源：http://sun.jinqigufen.top

Go:   resp.StatusCode
来源：http://skt.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://fxz.yj20258.top

C#:   (int)resp.StatusCode
来源：http://yft.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://tqs.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://shm.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://qdd.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ixm.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://seu.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zcy.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fzv.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dqt.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://flj.jinghuilouyu.cn

================================================================================
来源：http://wfi.xingfuxueyuan.xyz

M. 命令行 / 进程 / 环境
来源：http://oel.kuanghao11.cn

================================================================================
来源：http://uwn.meibo888.top

[M01] 读取命令行参数
来源：http://xuj.wangdashe.top

Py:   sys.argv[1:]
来源：http://qdp.wangdashe.top

PHP:  $argv;  $argc;
来源：http://kqo.daria6918.cn

JS:   process.argv.slice(2)
来源：http://amx.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://suh.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://zyi.aibaodan.cn

Go:   os.Args[1:]
来源：http://rox.cheryme.top

Ruby: ARGV
来源：http://uaw.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://rku.ehwqpu.com

[M02] 读取环境变量
来源：http://wgc.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://szb.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wrd.jlsjyb.cn

JS:   process.env.HOME
来源：http://hop.kuanghao11.cn

TS:   process.env.HOME
来源：http://kyd.yj20258888.top

Java: System.getenv("HOME")
来源：http://ils.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lgz.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://wcc.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pag.chenlongwang.top

[M03] 执行外部命令
来源：http://ctu.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ndn.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vmb.zdbjq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jbn.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nqz.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rxi.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vln.zhiwuduotai.top

Ruby: system("ls -l");  `ls -l`
来源：http://old.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://esb.dianchejie.cn

[M04] 获取当前工作目录
来源：http://kfx.tanke756.top

Py:   os.getcwd()
来源：http://abf.fehbvm.com

PHP:  getcwd();
来源：http://rlo.fanxiaobao.xyz

JS:   process.cwd()
来源：http://ooj.yongpay.top

TS:   process.cwd()
来源：http://yxv.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://kje.cucudq.cn

Go:   os.Getwd()
来源：http://upk.tanke756.top

Ruby: Dir.pwd
来源：http://xrx.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://cxc.hywenlv.cn

[M05] 设置退出码
来源：http://mtr.fehbvm.com

Py:   sys.exit(1)
来源：http://gwt.nwbrower.top

PHP:  exit(1);
来源：http://bol.fktsv.cn

JS:   process.exit(1)
来源：http://zkf.fzhhl.top

TS:   process.exit(1)
来源：http://nfr.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://xxp.zdqjudy.top

Go:   os.Exit(1)
来源：http://gwj.birdmap.top

Ruby: exit 1
来源：http://mbo.shangyingyoupin.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bjw.chenlongwang.top

[M06] 向标准错误输出
来源：http://zmn.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://lcm.sweek.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vbq.jianghu66.top

JS:   console.error("err")
来源：http://pbj.svipenyu.cn

TS:   console.error("err")
来源：http://tyt.fengsongda.top

Java: System.err.println("err")
来源：http://lgx.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ill.andypj.xyz

Ruby: warn "err"
来源：http://eyl.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://wmi.yongpay.top

[M07] 判断是否为主入口
来源：http://zzv.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://tok.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ehr.iojbl.cn

JS:   require.main === module
来源：http://wqg.xuanzx.com

TS:   require.main === module
来源：http://zth.jqgufenzy.top

Java: public static void main(String[] args)
来源：http://jmc.aizwys.cn

Go:   func main()
来源：http://zmr.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://utq.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://cpp.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://krx.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://inh.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://ljt.zycfv.cn

JS:   process.platform;  process.version
来源：http://lam.ybcxt.top

TS:   process.platform;  process.version
来源：http://bra.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qtd.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yoo.ctjpmb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ofk.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://jsn.daxiang520.top

================================================================================
来源：http://ckd.smart0.xyz

N. 数据结构与算法
来源：http://lii.ivvv.top

================================================================================
来源：http://ddj.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://rkn.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://nbb.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mih.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tfu.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lhm.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tvz.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://rnq.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dma.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://kem.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://sic.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://tts.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kam.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://cxw.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://sev.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://elz.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://iyi.sufxvd.cn

Ruby: arr.sort
来源：http://kha.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ltb.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://qki.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aty.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://jko.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nri.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ksi.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pin.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yai.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nno.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://caz.tianlin.xyz

[N04] 斐波那契数列
来源：http://zeq.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fjp.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rqe.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jsl.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jns.guowangkeji.top


<!-- 参考信息 -->