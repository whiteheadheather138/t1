代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://xtr.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qea.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zyd.shuidangran.top

[I05] 按正则拆分
来源：http://yrd.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lqw.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oto.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://inn.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://nyp.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://asd.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vzv.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mun.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gss.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://apt.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vlx.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://esf.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nhd.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mns.cqqwz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pbj.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mbf.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cxo.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jdm.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://uye.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ujm.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dwk.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ulo.zhaomingkeji.xyz

TS:   /error/gim
来源：http://ask.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://osr.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pjq.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://mdx.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cyg.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://mgr.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iwk.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cbw.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://akv.vehdjk.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iin.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://zsm.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vxj.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bue.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nxd.sxryk.cn

================================================================================
来源：http://xor.jinghuilouyu.cn

J. 日期与时间
来源：http://crd.nanxinkj.top

================================================================================
来源：http://jxq.ybcxt.top

[J01] 获取当前时间
来源：http://oun.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vof.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jdd.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://upn.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://hnj.feifeiyinyue.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hzp.316326.xyz

Go:   time.Now()
来源：http://nny.zhongyouzk.top

Ruby: Time.now
来源：http://qxg.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mww.yongpay.top

[J02] 格式化输出
来源：http://qnh.kuanghao11.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pag.ywan-chungtsiang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bez.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vzz.fzhhl.top

TS:   d.toISOString()
来源：http://jow.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yvr.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://och.hammf.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yyk.mhx1999.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eoq.daxiang520.top

[J03] 字符串解析为日期
来源：http://vxg.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://twl.sjlbkw.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://riw.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://jwo.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://ebz.svipenyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ypg.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gjc.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://moi.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mqe.yfazqb.com

[J04] 时间戳与日期互转
来源：http://yhr.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pvd.shanyushiyangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wca.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://asl.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lrt.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://quo.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ije.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gyv.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yhr.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://zei.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://ebw.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://sir.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iqj.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fkk.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://znx.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ftz.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://fqo.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://rmd.yanxiufei.cn

[J06] 计算两时间之差
来源：http://cog.pycfn.com

Py:   (end - start).total_seconds()
来源：http://tvs.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://upa.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zts.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://abj.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://fzl.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://jzl.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://dmm.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://qkh.sweek.top

[J07] 比较两个日期
来源：http://ntx.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://bot.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tuj.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://gmy.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hfp.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hky.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lhe.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://phz.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://pck.sxryk.cn

[J08] 提取年月日与星期
来源：http://exb.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uvz.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://naw.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zgq.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wlg.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ybw.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ylo.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hob.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bhd.jlsjyb.cn

[J09] 时区处理
来源：http://des.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bpz.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mac.gotoacloud.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kok.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rua.xylfe.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oxw.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vxf.ehwqpu.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dln.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eyj.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://rdm.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dag.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://imh.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uio.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dtm.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kek.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nuk.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oag.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://knw.c1oappe.top

================================================================================
来源：http://brv.52xcode.cn

K. JSON 与序列化
来源：http://mlv.jqgufenzy.top

================================================================================
来源：http://jrj.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://ycm.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qmz.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gmb.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://aek.uphjek.com

TS:   JSON.stringify(obj)
来源：http://esl.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vkp.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://epf.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://eet.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://oay.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://cbm.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://bay.sufxvd.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hos.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://miw.shuidangran.top

TS:   JSON.parse(s)
来源：http://gqy.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ins.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://ppa.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://ssf.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://esi.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://ytc.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mks.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zhb.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oxw.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://whh.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cli.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gxk.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://iop.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ylw.cashguo.top

[K04] 读取 JSON 文件
来源：http://bhb.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xwi.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dfp.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lsj.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ohu.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://duf.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wgl.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eid.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bzm.hysaishi.cn

[K05] 深拷贝对象
来源：http://eyd.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://hnm.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://pam.zhongyouzk.top

JS:   structuredClone(obj)
来源：http://lpp.shzxlz.cn

TS:   structuredClone(obj)
来源：http://vmn.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xrw.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pod.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zmn.cdnleiting.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uam.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://xsh.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lfb.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xfz.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jux.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dcv.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jse.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tdy.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aly.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rrd.sjlbkw.cn

[K07] 进制转换
来源：http://sle.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iji.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pml.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gkl.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wpi.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pwt.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nem.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ldh.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hgr.hesvh.cn

[K08] 二进制序列化（非 JSON）
来源：http://pxm.yuxming.cn

Py:   pickle.dumps(obj)
来源：http://hun.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uij.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://krd.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://bvx.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yje.sysykeji.top

Go:   encoding/gob
来源：http://iue.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://cwl.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bdp.pengpengdd.cyou

================================================================================
来源：http://rfe.ivvv.top

L. 网络请求
来源：http://ryw.52xcode.cn

================================================================================
来源：http://egq.daria6918.cn

[L01] 发送 GET 请求
来源：http://ulu.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dus.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gfu.jyoumei.cn

JS:   await fetch(url)
来源：http://muc.xuetiantiany.cn

TS:   await fetch(url)
来源：http://ekf.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rwr.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://hhf.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://mot.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://shp.ybcxt.top

[L02] 发送 POST JSON
来源：http://cio.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://wpt.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://obb.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mxu.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tfx.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vqq.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yzi.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xod.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jon.nanxinkj.top

[L03] 设置自定义请求头
来源：http://ogg.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vco.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nje.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nag.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fgo.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rmf.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ucb.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oxs.xylfe.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ydn.cucudq.cn

[L04] 设置超时
来源：http://kbr.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://ykg.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hkm.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pku.sysykeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fnm.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fjq.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dcl.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jxp.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oef.nwbrower.top

[L05] 上传文件（multipart）
来源：http://oyh.ppjwa.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fmk.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://caz.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mze.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jni.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zhy.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aff.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sgt.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mzq.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://nub.shanyushiyangtech.top

Py:   resp.json()
来源：http://mvt.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://cpi.0kj1m.cn

JS:   await resp.json()
来源：http://vcx.snrcjt.cn

TS:   await resp.json()
来源：http://wgp.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kfa.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dhp.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://kja.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iht.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://bpa.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dfk.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hxw.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://uju.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://cox.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://vly.dianchejie.cn

Go:   resp.StatusCode
来源：http://wqb.gogol.net.cn

Ruby: resp.code.to_i
来源：http://jrz.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://luq.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://ipf.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lcr.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://dtz.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fgb.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ada.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qhw.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://koh.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zpe.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hpc.cashguo.top

================================================================================
来源：http://rfi.ppjwa.cn

M. 命令行 / 进程 / 环境
来源：http://wvv.birdmap.top

================================================================================
来源：http://qsd.0kj1m.cn

[M01] 读取命令行参数
来源：http://bcc.pycfn.com

Py:   sys.argv[1:]
来源：http://gig.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://gnj.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://fzz.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://tct.meibo888.top

Java: args 数组（main 方法参数）
来源：http://fxf.yj20258888.top

Go:   os.Args[1:]
来源：http://zbi.dashuyun.cn

Ruby: ARGV
来源：http://xjk.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://ikm.yj20258888.top

[M02] 读取环境变量
来源：http://huw.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://upr.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://phr.feifeiyinyue.top

JS:   process.env.HOME
来源：http://epc.aibaodan.cn

TS:   process.env.HOME
来源：http://xuy.yj20258.top

Java: System.getenv("HOME")
来源：http://gdb.shzxlz.cn


<!-- 参考信息 -->