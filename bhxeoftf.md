代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sew.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zee.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://nke.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ffn.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://hku.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://ale.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bud.jqgufenzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vkh.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://zwn.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yzv.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xno.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://fsd.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://idk.c1oappe.top

[I03] 提取捕获分组
来源：http://cvc.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yxu.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mgh.ydzc1.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mci.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://khx.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uov.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xai.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://svb.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ukw.hongshengwenyu.top

[I04] 正则替换
来源：http://bgu.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://vzk.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jpo.yongpay.top

JS:   s.replace(/\d+/g, "#")
来源：http://jgk.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://dgn.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://ntz.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ucg.jqgfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gfr.xuetiantiany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ipr.xingfuxueyuan.xyz

[I05] 按正则拆分
来源：http://mbj.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qon.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eki.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://ywo.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://tya.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://dbr.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mzs.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mwv.cqqwz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ouk.nwbrower.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hxj.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sni.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ste.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pmz.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gqs.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cuu.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tmf.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rbn.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iii.cucudq.cn

[I07] 忽略大小写与多行模式
来源：http://tnx.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lmv.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cgw.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qzx.aibaodan.cn

TS:   /error/gim
来源：http://yiv.hnxiangtu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cow.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mbj.vehdjk.com

Ruby: s.scan(/error/i)
来源：http://dvo.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qma.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://pkk.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lzb.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dpy.snrcjt.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hts.xuetiantiany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zqw.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fif.c1oappe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xyl.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mij.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dei.yvedp.cn

================================================================================
来源：http://pwq.yanxiufei.cn

J. 日期与时间
来源：http://ggj.cdnleiting.top

================================================================================
来源：http://ubw.jlsjyb.cn

[J01] 获取当前时间
来源：http://cdw.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ltw.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hji.daria6918.cn

JS:   new Date();  Date.now()
来源：http://bxy.uphjek.com

TS:   new Date();  Date.now()
来源：http://ebj.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ass.hcnkem.com

Go:   time.Now()
来源：http://mro.sufxvd.cn

Ruby: Time.now
来源：http://wnk.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://adv.yuanzhike.top

[J02] 格式化输出
来源：http://oiw.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://trq.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://llj.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://soz.hesvh.cn

TS:   d.toISOString()
来源：http://mpz.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eph.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://szb.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mlk.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://etb.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://mrp.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jtu.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ivk.dashuyun.cn

JS:   new Date("2024-01-02")
来源：http://jcm.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://ksy.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://xst.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ayg.feifeiyinyue.top

Ruby: Date.parse("2024-01-02")
来源：http://sxx.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://syc.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://smg.andypj.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hbw.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mah.vqdsnc.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vlx.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jvc.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pde.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pqo.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://igd.fanxiaobao.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zgi.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://hgi.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://qkv.chenlongwang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lps.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eje.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ltt.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://azi.nwbrower.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wew.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://akw.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://wad.yuanzhike.top

[J06] 计算两时间之差
来源：http://mts.uphjek.com

Py:   (end - start).total_seconds()
来源：http://edg.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://mzz.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dzo.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fln.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://cih.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://axv.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://ajo.bbcook.cn

C#:   (end - start).TotalSeconds
来源：http://epb.yueranfly.top

[J07] 比较两个日期
来源：http://axb.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://qhb.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nlt.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vjf.jinqigufen.top

TS:   d1.getTime() < d2.getTime()
来源：http://wvn.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://whd.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gxk.chenlongwang.top

Ruby: d1 < d2;  d1 == d2
来源：http://buk.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://oon.yongpay.top

[J08] 提取年月日与星期
来源：http://ehf.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mrg.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vgc.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dkr.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ztj.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://epy.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ldh.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nou.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fht.fktsv.cn

[J09] 时区处理
来源：http://tig.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hxc.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tvy.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rkz.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rsp.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zuu.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sfi.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ozu.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://grk.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://vwp.cqqwz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jgd.wangdashe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gvw.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xfu.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cxj.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://onb.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://meh.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qvp.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mvr.ehwqpu.com

================================================================================
来源：http://ehm.pycfn.com

K. JSON 与序列化
来源：http://gji.aibaodan.cn

================================================================================
来源：http://bzu.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://vgj.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://err.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jrj.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://zyj.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://qtj.meibo888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yvy.jinghuilouyu.cn

Go:   json.Marshal(obj)
来源：http://nzi.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://osh.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://djs.zycfv.cn

[K02] JSON 字符串转对象
来源：http://xqw.mhx1999.top

Py:   json.loads(s)
来源：http://iwq.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zyd.jinqigfzy.top

JS:   JSON.parse(s)
来源：http://qfl.jianghu66.top

TS:   JSON.parse(s)
来源：http://zjz.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lok.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://rac.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://njo.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xmq.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://pqa.zdbjq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gng.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cdr.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://byq.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zwx.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wky.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fgy.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ewl.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fcu.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://hke.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qrf.havefunace.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pvd.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gqv.ydjk.org.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://umb.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ssz.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wpj.kuanghao11.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wdt.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://inc.daxiang520.top

[K05] 深拷贝对象
来源：http://iuj.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://bnc.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://xyd.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://hqa.aizwys.cn

TS:   structuredClone(obj)
来源：http://hmu.jqgufenzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rhy.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qai.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zmh.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lju.andypj.xyz

[K06] 解析 URL 查询串
来源：http://xuv.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wcm.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hbf.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axm.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oax.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nnp.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hmd.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uyc.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dvq.hfpthk.cn

[K07] 进制转换
来源：http://qke.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vwh.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://isp.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cgg.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://shn.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qat.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ift.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wbu.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ozx.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://azf.redwolf501.top

Py:   pickle.dumps(obj)
来源：http://awu.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jwn.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://rnd.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://zcc.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fel.sjlbkw.cn

Go:   encoding/gob
来源：http://lje.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://wuv.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ovn.nanxuanxn.top

================================================================================
来源：http://cqw.jiagoushi.top

L. 网络请求
来源：http://pgx.andypj.xyz

================================================================================
来源：http://wti.uphjek.com

[L01] 发送 GET 请求
来源：http://vlf.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dsl.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vye.hammf.cn

JS:   await fetch(url)
来源：http://xjx.zdbjq.cn

TS:   await fetch(url)
来源：http://uth.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wtb.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://mhi.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ceq.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://shr.guowangkeji.top

[L02] 发送 POST JSON
来源：http://ztb.yj202588.top

Py:   requests.post(url, json={"a": 1})
来源：http://ghf.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cqm.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mqp.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fsu.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vsa.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pnz.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jkr.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://llt.fzhhl.top

[L03] 设置自定义请求头
来源：http://qoi.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://abc.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rxe.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cfc.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zma.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cqa.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mav.wangshuangyany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sol.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mxi.guowangkeji.top

[L04] 设置超时
来源：http://avd.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://kec.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://erk.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ecd.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kai.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ltb.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ivw.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nuk.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rrk.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://pec.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iym.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ady.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://als.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lkl.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dny.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dih.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xlo.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xdf.xuanzx.com

[L06] 解析响应为 JSON
来源：http://zzm.52xcode.cn

Py:   resp.json()
来源：http://umj.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://dgz.gogol.net.cn

JS:   await resp.json()
来源：http://tkl.hongshengwenyu.top

TS:   await resp.json()
来源：http://qal.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qte.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lwr.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://zhh.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lsb.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://xfi.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ohd.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ydx.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://qzx.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://qnn.yanxiufei.cn

Java: resp.statusCode()
来源：http://jjn.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://aet.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://xtp.chenzaomai.com


<!-- 参考信息 -->