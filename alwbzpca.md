代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wvj.pycfn.com

[I03] 提取捕获分组
来源：http://kvm.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eja.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bnr.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gtm.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://imj.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rdt.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dqx.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mif.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aep.cucudq.cn

[I04] 正则替换
来源：http://woy.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hio.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lnz.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://aal.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hnc.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ywg.hammf.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://abf.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uvc.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://run.iojbl.cn

[I05] 按正则拆分
来源：http://ihr.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oek.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rvs.kuanghao11.cn

JS:   s.split(/\s*,\s*/)
来源：http://adn.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://ubv.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://bzs.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hzz.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xpb.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cvy.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qhy.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lnv.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jxf.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://azq.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vsc.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ucw.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eie.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zbe.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://onr.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://sgd.wangdashe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rzz.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://loi.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://urn.daria6918.cn

TS:   /error/gim
来源：http://ryq.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ggv.kuanghao11.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://umw.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://uqi.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sdh.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://wbd.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tqz.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ddy.bjfxy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mdy.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qto.vehdjk.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://djc.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cez.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yrc.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tkn.zhaomingkeji.xyz

================================================================================
来源：http://fhs.ydjk.org.cn

J. 日期与时间
来源：http://reb.ywan-chungtsiang.top

================================================================================
来源：http://ejv.ehwqpu.com

[J01] 获取当前时间
来源：http://wtu.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ilw.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fyz.tian-w.cn

JS:   new Date();  Date.now()
来源：http://non.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://yai.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cwd.hnxiangtu.top

Go:   time.Now()
来源：http://xnt.nanxuanxn.top

Ruby: Time.now
来源：http://hhv.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pzp.yangfankeji.com

[J02] 格式化输出
来源：http://kto.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://atn.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aqb.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cci.zycfv.cn

TS:   d.toISOString()
来源：http://hbu.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hxa.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kgf.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fjk.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fzc.yuanzhike.top

[J03] 字符串解析为日期
来源：http://vrp.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lyt.zhaomingkeji.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gjn.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://jjm.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://fno.hongshengwenyu.top

Java: LocalDate.parse("2024-01-02")
来源：http://onp.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://djm.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://egv.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hwj.xuanzx.com

[J04] 时间戳与日期互转
来源：http://nru.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ilj.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://swt.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://weo.vqdsnc.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://urx.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://igc.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nej.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://edv.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xos.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://bcj.uphjek.com

Py:   now + timedelta(days=7)
来源：http://niz.shzxlz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hhj.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rhf.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://srb.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://izy.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://myw.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://pqi.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://vul.vqdsnc.cn

[J06] 计算两时间之差
来源：http://ixh.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://prr.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://vwk.jqgufenzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ckw.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cwf.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://roy.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://nhz.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://dis.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://top.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://num.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://nqg.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uwo.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://bkb.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://hrb.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mjn.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aua.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://zzo.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://yhs.jianghu66.top

[J08] 提取年月日与星期
来源：http://uxi.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lwm.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zpr.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zyv.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hyv.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pzx.jyoumei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sia.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rjh.shzxlz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dtq.gogol.net.cn

[J09] 时区处理
来源：http://zzw.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xfg.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dba.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cfx.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ifo.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bgq.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xsp.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lap.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xkr.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://get.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://nyn.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://isv.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kwd.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ryy.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zif.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ask.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sli.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ggb.yongpay.top

================================================================================
来源：http://wte.wangshuangyany.cn

K. JSON 与序列化
来源：http://pox.jiagoushi.top

================================================================================
来源：http://mvf.ctjpmb.com

[K01] 对象转 JSON 字符串
来源：http://ofc.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dav.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ljd.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://bvl.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://epz.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://igm.daria6918.cn

Go:   json.Marshal(obj)
来源：http://stg.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gwh.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://chn.pycfn.com

[K02] JSON 字符串转对象
来源：http://wnd.ydjk.org.cn

Py:   json.loads(s)
来源：http://ebj.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wdo.jianghu66.top

JS:   JSON.parse(s)
来源：http://kji.wangshuangyany.cn

TS:   JSON.parse(s)
来源：http://lmq.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://obt.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://hpy.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://cxv.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hzl.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://pvx.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fif.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tvj.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://rzx.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ryb.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dtq.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wlq.dashuyun.cn

Ruby: JSON.pretty_generate(obj)
来源：http://txb.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yjq.tian-w.cn

[K04] 读取 JSON 文件
来源：http://wmh.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jch.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://elo.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwq.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oou.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fbo.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ebi.sxryk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uft.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lzm.shuidangran.top

[K05] 深拷贝对象
来源：http://ign.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://dnn.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://xcc.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://tre.snrcjt.cn

TS:   structuredClone(obj)
来源：http://cdl.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mzj.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fbz.cqqwz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://off.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qlz.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://vwo.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gvd.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kmg.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uhz.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pih.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yuq.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qfh.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ykg.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dbm.shanyushiyangkeji.top

[K07] 进制转换
来源：http://npi.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xtq.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mhd.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ych.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cnt.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zdr.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ikr.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vee.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://irq.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://vdz.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://ggt.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qwy.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://gln.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://fzm.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eok.9152youxi.cn

Go:   encoding/gob
来源：http://xau.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://pjt.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zxg.jlsjyb.cn

================================================================================
来源：http://oac.xuetiantiany.cn

L. 网络请求
来源：http://seb.hysaishi.cn

================================================================================
来源：http://egn.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://bbc.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zqz.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zjw.hnxiangtu.top

JS:   await fetch(url)
来源：http://oix.zhengqikj.top

TS:   await fetch(url)
来源：http://xwd.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qzl.ydjk.org.cn

Go:   resp, err := http.Get(url)
来源：http://oij.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://udj.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://thq.sysykeji.top

[L02] 发送 POST JSON
来源：http://hgt.bbcook.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fqq.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fhb.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lxy.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wcq.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bxe.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hat.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ehp.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ybq.yj20258888.top

[L03] 设置自定义请求头
来源：http://njd.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vkq.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mfp.zdqjudy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wwy.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tuy.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uzh.tanke756.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ivw.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iql.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fqh.vqdsnc.cn

[L04] 设置超时
来源：http://ivg.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://pic.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ewp.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xgw.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qnn.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nmd.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cgr.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ypq.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bey.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://izl.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zew.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kra.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mid.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hiv.bjfxy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ynd.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vcn.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://alr.ctjpmb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ofq.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://npj.pycfn.com

Py:   resp.json()
来源：http://kor.shuidangran.top

PHP:  json_decode($body, true);
来源：http://bnc.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://uji.shanyushiyangtech.top

TS:   await resp.json()
来源：http://koy.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zaw.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gvj.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://hiw.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rxa.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://dfg.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://goj.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zpq.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://hbi.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://efx.shuidangran.top

Java: resp.statusCode()
来源：http://gfl.ydjk.org.cn

Go:   resp.StatusCode
来源：http://ixh.zhengqikj.top

Ruby: resp.code.to_i
来源：http://pel.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://ybf.smart0.xyz

[L08] 并发请求多个地址
来源：http://iri.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ayt.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://cqm.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ozq.0kj1m.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vxe.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wuf.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qzm.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ccu.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://asz.ehwqpu.com

================================================================================
来源：http://vcu.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://mnc.xinyue.icu


<!-- 参考信息 -->