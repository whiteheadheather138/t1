代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hyq.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qcn.yuxming.cn

[I04] 正则替换
来源：http://rbb.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://skl.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lyh.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://jfz.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://ulq.daria6918.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cyh.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zpz.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://pmg.cucudq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://swz.jianghu66.top

[I05] 按正则拆分
来源：http://oab.tanke756.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bub.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://teu.aibaodan.cn

JS:   s.split(/\s*,\s*/)
来源：http://jsz.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://znp.shanyushiyangtech.top

Java: s.split("\\s*,\\s*")
来源：http://ldk.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://frd.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vnt.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oly.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rmb.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yhw.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vwh.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lsr.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jlf.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eht.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zrr.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fud.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://krc.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://rpe.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nqu.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nzx.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zed.hongshengwenyu.top

TS:   /error/gim
来源：http://buv.sufxvd.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rsm.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dor.sweek.top

Ruby: s.scan(/error/i)
来源：http://ubd.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wga.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://zuz.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gpp.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hkb.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://phc.shzxlz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eui.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zmw.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nja.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sep.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wwr.yj20258.top

================================================================================
来源：http://kkd.chenlongwang.top

J. 日期与时间
来源：http://ifr.dianchejie.cn

================================================================================
来源：http://aai.gogol.net.cn

[J01] 获取当前时间
来源：http://huj.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://wjh.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zru.dashuyun.cn

JS:   new Date();  Date.now()
来源：http://iwa.smart0.xyz

TS:   new Date();  Date.now()
来源：http://jmx.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nkg.chenzaomai.com

Go:   time.Now()
来源：http://loh.jyoumei.cn

Ruby: Time.now
来源：http://rgl.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ayr.jqgufenzy.top

[J02] 格式化输出
来源：http://qfx.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rlf.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ssd.daria6918.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kyb.daxiang520.top

TS:   d.toISOString()
来源：http://eso.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tpo.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://naa.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hgb.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://obg.zdbjq.cn

[J03] 字符串解析为日期
来源：http://vzd.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xje.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ybe.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://rzs.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://bhy.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://dgt.zhoulong.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ckb.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://wne.yongpay.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nuw.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://gfj.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jgp.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wbu.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://quy.quarkkingdee.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ikq.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qgz.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oux.zhixingplan.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vbw.hywenlv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://icl.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://zxi.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://dhb.c1oappe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://off.yfazqb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jwc.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://egt.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://hrq.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jvx.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://vwg.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://gqp.birdmap.top

[J06] 计算两时间之差
来源：http://adg.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://gnr.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://ktp.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ihp.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rqg.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://qyo.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://ctx.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://cet.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://wkg.9152youxi.cn

[J07] 比较两个日期
来源：http://qse.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://fxq.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yaa.ydzc1.top

JS:   d1.getTime() < d2.getTime()
来源：http://qzb.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ovo.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ysk.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://arw.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cpc.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://opl.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://hvj.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wtw.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nho.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uhr.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://une.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qkk.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rrt.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ujo.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fru.haohaochexian.top

[J09] 时区处理
来源：http://wrt.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wql.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://csp.birdmap.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wmy.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cuw.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fth.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sjg.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hjk.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zuy.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://ole.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tzw.tian-w.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yxi.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xxz.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://buf.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hvr.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ynp.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ssc.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pzl.hesvh.cn

================================================================================
来源：http://dtf.hnqzz.top

K. JSON 与序列化
来源：http://fpm.jlsjyb.cn

================================================================================
来源：http://ovr.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://esl.gzhubu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nqb.yvedp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ehc.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://ejs.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://sze.tianlin.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kbk.xylfe.cn

Go:   json.Marshal(obj)
来源：http://fwc.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fpr.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://mvw.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://dfo.yfazqb.com

Py:   json.loads(s)
来源：http://cgd.jqgfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lkz.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://aty.zhixingplan.top

TS:   JSON.parse(s)
来源：http://hra.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fcv.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://dxz.yuxming.cn

Ruby: JSON.parse(s)
来源：http://vfo.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://chy.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://vnw.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yyd.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gyl.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ibu.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zwk.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lpr.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zye.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://knq.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nmk.yuxming.cn

[K04] 读取 JSON 文件
来源：http://ezq.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://njf.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eqj.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nmr.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rsp.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nor.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ago.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wnv.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rpe.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://ndi.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://avp.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://dgn.pycfn.com

JS:   structuredClone(obj)
来源：http://szq.fzhhl.top

TS:   structuredClone(obj)
来源：http://pos.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bid.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://njz.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rmn.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qnn.redwolf501.top

[K06] 解析 URL 查询串
来源：http://tyb.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lxm.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nmo.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pxl.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gbs.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://heh.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dfi.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qhr.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xdz.shzxlz.cn

[K07] 进制转换
来源：http://eer.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rqb.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gmu.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zjz.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://omz.mhx1999.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dah.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jqa.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://teq.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wzy.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://hbg.jianghu66.top

Py:   pickle.dumps(obj)
来源：http://puu.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://unw.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://yxh.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://lus.9152youxi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rfo.iojbl.cn

Go:   encoding/gob
来源：http://ehf.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://xie.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vsj.zhijiandao.cn

================================================================================
来源：http://ixu.yongpay.top

L. 网络请求
来源：http://biu.sweek.top

================================================================================
来源：http://mig.fengsongda.top

[L01] 发送 GET 请求
来源：http://hmf.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ide.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://loi.aibaodan.cn

JS:   await fetch(url)
来源：http://ywf.feifeiyinyue.top

TS:   await fetch(url)
来源：http://sef.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mak.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://dqh.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bbc.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kpk.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://jxp.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://tlg.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lkx.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rgi.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://set.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://giq.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vip.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kzc.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cyb.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://bil.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xxf.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://frq.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lsw.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cik.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ydd.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ybb.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xdi.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cpk.hfpthk.cn

[L04] 设置超时
来源：http://xqr.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://jnk.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ouc.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rxx.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://leq.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gko.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ieh.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oqv.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hpy.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://gpj.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://irp.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uhl.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aaz.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://evo.bbcook.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qwy.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pqe.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rjs.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://edj.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://wpb.xylfe.cn

Py:   resp.json()
来源：http://wvu.nwbrower.top

PHP:  json_decode($body, true);
来源：http://eln.sjlbkw.cn

JS:   await resp.json()
来源：http://orw.sjlbkw.cn

TS:   await resp.json()
来源：http://zmf.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pzv.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jpa.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://cbs.hcnkem.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gdj.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://jjn.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vfe.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dei.0kj1m.cn

JS:   resp.ok;  resp.status
来源：http://ruf.ivvv.top

TS:   resp.ok;  resp.status
来源：http://qno.daria6918.cn

Java: resp.statusCode()
来源：http://ihr.svipenyu.cn

Go:   resp.StatusCode
来源：http://jlu.jinqigufen.top

Ruby: resp.code.to_i
来源：http://fbd.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://bvm.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://pwd.yj20258888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mvd.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://fyc.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yza.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lke.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nko.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ovx.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cbs.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mcd.zhijiandao.cn

================================================================================
来源：http://ovj.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://lqx.nanxuanxn.top

================================================================================
来源：http://awq.0kj1m.cn

[M01] 读取命令行参数
来源：http://isp.tian-w.cn

Py:   sys.argv[1:]
来源：http://kib.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://rux.jianghu66.top

JS:   process.argv.slice(2)
来源：http://txr.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://flh.yueranfly.top

Java: args 数组（main 方法参数）
来源：http://lcu.epnwcf.com

Go:   os.Args[1:]
来源：http://vdd.jqgufenzy.top


<!-- 参考信息 -->