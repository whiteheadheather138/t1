代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ywp.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://dqg.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vis.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gda.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mcv.cdnleiting.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fdi.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jea.xylfe.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://duv.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zea.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xub.0kj1m.cn

[I04] 正则替换
来源：http://rlw.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jgx.sysykeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dly.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://orq.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://eab.hesvh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bwe.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qte.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jfq.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://shi.hnxiangtu.top

[I05] 按正则拆分
来源：http://mir.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pqy.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sul.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://yoa.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://aey.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://hzz.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://prw.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ggb.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lsx.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zke.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dgl.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gxf.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qvj.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpn.jqgufenzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tzl.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tgu.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ipw.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wjy.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://fyj.tianlin.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wls.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lxs.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vue.fanxiaobao.xyz

TS:   /error/gim
来源：http://hgx.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ckd.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ipx.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://rnm.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://llo.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://kvg.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ukr.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pmi.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oig.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xiv.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://unb.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://utn.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yyo.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mke.birdmap.top

================================================================================
来源：http://vzi.tian-w.cn

J. 日期与时间
来源：http://gwc.zhixingplan.top

================================================================================
来源：http://fvy.hongshengwenyu.top

[J01] 获取当前时间
来源：http://ofz.cashguo.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pee.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jlx.zycfv.cn

JS:   new Date();  Date.now()
来源：http://bfo.yj202588.top

TS:   new Date();  Date.now()
来源：http://ucx.shzxlz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://knt.guannengcc.top

Go:   time.Now()
来源：http://wby.daxiang520.top

Ruby: Time.now
来源：http://xfk.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mfz.yvedp.cn

[J02] 格式化输出
来源：http://abj.nanxinkj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cdi.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hjo.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ymd.aibaodan.cn

TS:   d.toISOString()
来源：http://sjc.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vqp.cashguo.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tzd.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oyx.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gwb.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://ouf.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rfu.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qug.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://tbc.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://rsp.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://xhp.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gxv.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://fmo.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ycz.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://gcu.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qpv.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vkg.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jiz.jianghu66.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mys.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mhg.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://npr.tarul.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ffe.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cig.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://ooq.aibaodan.cn

Py:   now + timedelta(days=7)
来源：http://iot.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://asv.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wtu.zhoulong.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://urf.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://obi.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mmb.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://avd.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ibz.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://ppk.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://mov.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://gug.epnwcf.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xuu.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qnh.yvedp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tjm.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://qhl.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://jph.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://obm.hcnkem.com

[J07] 比较两个日期
来源：http://zqp.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://ftv.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vms.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://qbg.daxiang520.top

TS:   d1.getTime() < d2.getTime()
来源：http://cwn.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jvq.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ttz.hongshengwenyu.top

Ruby: d1 < d2;  d1 == d2
来源：http://pzp.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://sqy.shzxlz.cn

[J08] 提取年月日与星期
来源：http://xin.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ihx.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eby.sjlbkw.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dyz.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nvu.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ndk.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rxa.chenjidiqi.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wtp.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tij.birdmap.top

[J09] 时区处理
来源：http://lqo.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ikb.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tnr.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vtn.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zyt.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mks.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oht.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tkk.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lot.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://mlv.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qqp.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wrw.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ltn.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uqo.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xxc.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zuj.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://snd.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfh.shanyushiyangkeji.top

================================================================================
来源：http://oiu.xinyue.icu

K. JSON 与序列化
来源：http://pex.shangyingyoupin.top

================================================================================
来源：http://gbk.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://krb.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lub.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rbv.zhoulong.xyz

JS:   JSON.stringify(obj)
来源：http://pwi.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://qri.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sqv.iojbl.cn

Go:   json.Marshal(obj)
来源：http://bkm.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://mlu.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://gbk.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://flg.feifeiyinyue.top

Py:   json.loads(s)
来源：http://vxw.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nft.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://lfk.yvedp.cn

TS:   JSON.parse(s)
来源：http://hkb.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lfx.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://itx.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://fgv.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tlf.jlsjyb.cn

[K03] JSON 美化输出（带缩进）
来源：http://ngi.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hgz.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://txd.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zeu.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tps.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wny.guowangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xbh.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://upi.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kvg.yueranfly.top

[K04] 读取 JSON 文件
来源：http://aro.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xkb.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gdy.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ivk.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yxs.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sut.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://goo.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://okw.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cbf.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://ksp.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://jgr.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://fsf.haohaochexian.top

JS:   structuredClone(obj)
来源：http://xzw.yangfankeji.com

TS:   structuredClone(obj)
来源：http://ivz.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ouf.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gme.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ndm.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cug.gzhubu.top

[K06] 解析 URL 查询串
来源：http://fbc.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sxi.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xix.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tia.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ajr.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ubi.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yhf.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://swr.cheryme.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wfh.jinyuanbaomall.cn

[K07] 进制转换
来源：http://axm.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qei.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rnm.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hak.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qmg.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kwq.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xsa.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ptj.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jfm.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://gcd.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://kiv.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://wmx.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://mcj.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://qey.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oyt.zdbjq.cn

Go:   encoding/gob
来源：http://gyz.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://hyo.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vhs.jyoumei.cn

================================================================================
来源：http://dxq.chenlongwang.top

L. 网络请求
来源：http://bub.yueranfly.top

================================================================================
来源：http://vlu.uphjek.com

[L01] 发送 GET 请求
来源：http://otx.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://goo.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pqp.jqgfzy.top

JS:   await fetch(url)
来源：http://imr.andypj.xyz

TS:   await fetch(url)
来源：http://ctd.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cki.kuanghao11.cn

Go:   resp, err := http.Get(url)
来源：http://rjx.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lwk.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wvc.yueranfly.top

[L02] 发送 POST JSON
来源：http://zbb.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://npq.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ucv.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zjc.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xup.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mhi.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hvb.zhaomingkeji.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hiz.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cuh.hywenlv.cn

[L03] 设置自定义请求头
来源：http://edv.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://coh.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ogo.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dym.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://onp.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zgn.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uim.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qch.feifeiyinyue.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rji.zycfv.cn

[L04] 设置超时
来源：http://osk.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://rdj.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hfw.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wkp.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zok.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://paz.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aih.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zwj.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://whp.ybcxt.top

[L05] 上传文件（multipart）
来源：http://whl.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sti.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uty.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://laj.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hei.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eoy.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gfm.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://non.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xph.cheryme.top

[L06] 解析响应为 JSON
来源：http://tvs.jinqigfzy.top

Py:   resp.json()
来源：http://yzz.iojbl.cn

PHP:  json_decode($body, true);
来源：http://xno.wangshuangyany.cn

JS:   await resp.json()
来源：http://tkg.jinghuilouyu.cn

TS:   await resp.json()
来源：http://wcw.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cns.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://omx.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://dog.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tcc.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://brg.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wvk.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bpu.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://mvg.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://sjn.sjlbkw.cn

Java: resp.statusCode()
来源：http://dmd.hnxiangtu.top

Go:   resp.StatusCode
来源：http://vab.guannengcc.top

Ruby: resp.code.to_i
来源：http://tns.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://fdf.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://xzd.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ksk.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://qkt.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ara.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jnx.bjfxy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ful.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wxo.tanke756.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dqa.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://szs.yj20258.top

================================================================================
来源：http://ncr.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://ezz.fanxiaobao.xyz


<!-- 参考信息 -->