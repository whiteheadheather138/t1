代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pkz.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://tlo.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zjj.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bns.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nup.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cha.uphjek.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xgr.dashuyun.cn

[I05] 按正则拆分
来源：http://dpa.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fnt.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zez.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://rea.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://yem.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://eas.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gwo.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nli.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://irs.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sxz.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wrh.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://daw.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qnq.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fhu.xuanzx.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nld.yj202588.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vyd.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xrs.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://krc.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://nwg.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jme.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jrt.hywenlv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rjb.andypj.xyz

TS:   /error/gim
来源：http://nkt.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://owt.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yld.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://rys.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://flo.andypj.xyz

[I08] 贪婪与非贪婪匹配
来源：http://jtd.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ujt.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mak.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sya.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bnb.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://bcf.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://leh.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ldp.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://njs.havefunace.top

================================================================================
来源：http://qgr.yj202588.top

J. 日期与时间
来源：http://slt.zhijiandao.cn

================================================================================
来源：http://ynu.shuidangran.top

[J01] 获取当前时间
来源：http://hzo.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://apl.fehbvm.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yhf.fzhhl.top

JS:   new Date();  Date.now()
来源：http://hds.tarul.cn

TS:   new Date();  Date.now()
来源：http://ovh.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jdu.nanxinkj.top

Go:   time.Now()
来源：http://nxd.zycfv.cn

Ruby: Time.now
来源：http://dyk.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jxk.hywenlv.cn

[J02] 格式化输出
来源：http://hhi.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rho.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nfa.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xpu.sjlbkw.cn

TS:   d.toISOString()
来源：http://qce.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zts.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://shr.havefunace.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qkn.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cpu.uphjek.com

[J03] 字符串解析为日期
来源：http://jjw.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yox.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://szk.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://gxs.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://knn.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://kov.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://myp.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://blx.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ice.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://nbv.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pxt.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cqy.zhixingplan.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xya.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://bpy.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jiq.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nrn.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xop.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rcc.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://gpt.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://bre.mhx1999.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ama.52xcode.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rhi.yvedp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xkn.cqqwz.cn

Java: LocalDate.now().plusDays(7)
来源：http://vyo.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ttj.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://ftz.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://cpt.jinqigufen.top

[J06] 计算两时间之差
来源：http://hri.daxiang520.top

Py:   (end - start).total_seconds()
来源：http://yrj.ehwqpu.com

PHP:  $end->diff($start)->days;
来源：http://iqa.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rqs.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kjc.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://fuw.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://wqv.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://kyi.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://syk.sufxvd.cn

[J07] 比较两个日期
来源：http://inw.daria6918.cn

Py:   d1 < d2;  d1 == d2
来源：http://qkw.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pbi.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://dmd.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://kai.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eth.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lsl.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://maw.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://qis.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://jil.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ttk.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ucj.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kjm.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iso.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hme.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ddo.nwbrower.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://diz.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ppb.jlsjyb.cn

[J09] 时区处理
来源：http://uvo.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zva.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mul.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sng.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wrf.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tjd.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ooi.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ipa.snrcjt.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://viz.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://axn.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gtw.cucudq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://upo.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ceq.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kpg.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ydh.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hwi.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bwe.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mdg.hnxiangtu.top

================================================================================
来源：http://yzv.daxiang520.top

K. JSON 与序列化
来源：http://adi.yvedp.cn

================================================================================
来源：http://wwq.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://igo.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rpc.cdnleiting.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://frh.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://oao.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://gjz.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ljy.ydzc1.top

Go:   json.Marshal(obj)
来源：http://vbx.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oqu.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://akp.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://mke.52xcode.cn

Py:   json.loads(s)
来源：http://dos.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qix.cucudq.cn

JS:   JSON.parse(s)
来源：http://fzc.ehwqpu.com

TS:   JSON.parse(s)
来源：http://blz.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dsd.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://uli.meibo888.top

Ruby: JSON.parse(s)
来源：http://ity.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zxj.cucudq.cn

[K03] JSON 美化输出（带缩进）
来源：http://yki.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bmf.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xfx.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tsf.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://msg.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oij.quarkkingdee.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yyi.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://czo.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nfo.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://msx.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pme.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qlx.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gvu.yj20258888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dlj.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ltt.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qlx.kuanghao11.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ujl.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ryu.ybcxt.top

[K05] 深拷贝对象
来源：http://lln.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://equ.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://qfk.yongpay.top

JS:   structuredClone(obj)
来源：http://bxs.snrcjt.cn

TS:   structuredClone(obj)
来源：http://fqi.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jbz.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tjd.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://din.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tdo.wangdashe.top

[K06] 解析 URL 查询串
来源：http://vfd.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xay.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vcc.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fuy.wangdashe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pis.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://avi.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cvf.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://adh.316326.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gfo.aizwys.cn

[K07] 进制转换
来源：http://two.zhijiandao.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ral.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mbj.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://evn.hesvh.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xsg.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wrw.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rpt.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qei.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rzh.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://jfp.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://zcd.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ift.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://tyn.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://kpi.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iun.0kj1m.cn

Go:   encoding/gob
来源：http://jwx.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://rur.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wsh.hnqzz.top

================================================================================
来源：http://ccy.tanke756.top

L. 网络请求
来源：http://sre.pengpengdd.cyou

================================================================================
来源：http://whw.aibaodan.cn

[L01] 发送 GET 请求
来源：http://uqy.ehwqpu.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sga.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rqq.ydjk.org.cn

JS:   await fetch(url)
来源：http://gub.zdqjudy.top

TS:   await fetch(url)
来源：http://zwk.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pwi.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://dep.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xba.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ixw.tanke756.top

[L02] 发送 POST JSON
来源：http://cnz.ctjpmb.com

Py:   requests.post(url, json={"a": 1})
来源：http://epj.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zyo.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://etg.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qwq.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://anu.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pzg.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nqv.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vfm.smart0.xyz

[L03] 设置自定义请求头
来源：http://qjg.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://agv.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bor.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fwg.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ckm.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://elw.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uoi.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hrd.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lap.kuanghao11.cn

[L04] 设置超时
来源：http://tyo.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://qzb.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jpo.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fyu.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://maw.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vuh.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bvi.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://krv.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://apc.ydzc1.top

[L05] 上传文件（multipart）
来源：http://nrb.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bjl.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://paw.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://env.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xpa.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nzb.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://acj.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wwn.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wpt.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://qhv.wangdashe.top

Py:   resp.json()
来源：http://hvd.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://zsn.snrcjt.cn

JS:   await resp.json()
来源：http://pnx.9152youxi.cn

TS:   await resp.json()
来源：http://vnl.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fec.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bxx.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://csz.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oqm.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://cak.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://czy.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ueq.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://yoy.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://kck.pycfn.com

Java: resp.statusCode()
来源：http://few.sysykeji.top

Go:   resp.StatusCode
来源：http://jet.yj20258888.top

Ruby: resp.code.to_i
来源：http://aud.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://efi.ehwqpu.com

[L08] 并发请求多个地址
来源：http://lzr.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rte.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://alg.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ryb.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yhe.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bih.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sru.cdnleiting.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jcy.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://srl.aizwys.cn

================================================================================
来源：http://zip.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://cqz.sufxvd.cn

================================================================================
来源：http://kro.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://sov.c1oappe.top

Py:   sys.argv[1:]
来源：http://pgk.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://xdt.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://kek.bjfxy.top

TS:   process.argv.slice(2)
来源：http://arf.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://kog.fehbvm.com

Go:   os.Args[1:]
来源：http://mxh.zdbjq.cn

Ruby: ARGV
来源：http://qhj.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://usz.yj20258.top

[M02] 读取环境变量
来源：http://teu.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://bmf.shzxlz.cn


<!-- 参考信息 -->