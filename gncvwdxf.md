代发 wailian999

[I02] 提取所有匹配
来源：http://bzj.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://oyj.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mak.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://swm.fzhhl.top

TS:   s.match(/\d+/g)
来源：http://srj.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kjs.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pwl.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://cwy.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qcb.52xcode.cn

[I03] 提取捕获分组
来源：http://xxi.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kmr.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://crb.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zsb.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jkj.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rjd.ivvv.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gbf.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ttz.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wkg.aizwys.cn

[I04] 正则替换
来源：http://lfz.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://uwv.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ycz.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fri.cqqwz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qjs.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://udl.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://izk.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nnz.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oow.fehbvm.com

[I05] 按正则拆分
来源：http://rgf.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cwb.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://edm.sufxvd.cn

JS:   s.split(/\s*,\s*/)
来源：http://tot.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://aiv.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://hhj.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wwx.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jej.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ero.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wny.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iqs.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ucl.tarul.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lby.wangshuangyany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jkt.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://utd.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qzf.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pok.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://drz.nwbrower.top

[I07] 忽略大小写与多行模式
来源：http://aye.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jpw.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jzt.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kto.andypj.xyz

TS:   /error/gim
来源：http://hcr.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nsd.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zbc.sweek.top

Ruby: s.scan(/error/i)
来源：http://qqw.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jfn.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://mek.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zqj.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vus.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mpd.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rlz.yonumen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nqj.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gti.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kgj.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://izu.fzhhl.top

================================================================================
来源：http://kyd.xylfe.cn

J. 日期与时间
来源：http://vgl.svipenyu.cn

================================================================================
来源：http://iai.jinqigufen.top

[J01] 获取当前时间
来源：http://qqi.fzhhl.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vjm.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ojq.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://foy.c1oappe.top

TS:   new Date();  Date.now()
来源：http://zuc.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://kbh.cheryme.top

Go:   time.Now()
来源：http://kki.birdmap.top

Ruby: Time.now
来源：http://lya.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qrk.hysaishi.cn

[J02] 格式化输出
来源：http://ipn.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vml.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zfx.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ahq.quarkkingdee.top

TS:   d.toISOString()
来源：http://wgv.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hdt.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vgn.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://loj.ydzc1.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://exo.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://mdt.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qlf.0kj1m.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bsc.yj202588.top

JS:   new Date("2024-01-02")
来源：http://ftv.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://gfy.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://gyk.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ibl.nanxuanxn.top

Ruby: Date.parse("2024-01-02")
来源：http://jbt.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xnw.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://xjs.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fiw.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rwr.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jlk.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://svc.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mnz.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xdj.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vgm.andypj.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ksx.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://qnz.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://srl.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rmv.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://enr.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://axp.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://rsp.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xkq.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://vkk.tian-w.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ovr.sjlbkw.cn

[J06] 计算两时间之差
来源：http://fut.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://zfc.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://nld.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cwn.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://znz.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://krf.tarul.cn

Go:   end.Sub(start).Hours()
来源：http://aud.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://dyv.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://fav.jinqigfzy.top

[J07] 比较两个日期
来源：http://net.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://xih.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cmm.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://tef.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://mnx.yueranfly.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://luc.zycfv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ire.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bcb.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://dqi.yj20258.top

[J08] 提取年月日与星期
来源：http://mpv.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mlg.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://juv.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pgb.redwolf501.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nrd.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fvp.yvedp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://czi.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yke.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sma.yangfankeji.com

[J09] 时区处理
来源：http://cab.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dag.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kqb.hywenlv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mnl.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mju.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wty.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bts.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qzb.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rbr.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://iap.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nrg.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tuk.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wna.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://npd.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dfj.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mhg.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nnv.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bsl.gogol.net.cn

================================================================================
来源：http://hpu.zhoulong.xyz

K. JSON 与序列化
来源：http://ien.gotoacloud.top

================================================================================
来源：http://npo.wangdashe.top

[K01] 对象转 JSON 字符串
来源：http://vwd.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cpy.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uwk.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://xun.zdqjudy.top

TS:   JSON.stringify(obj)
来源：http://eig.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://igl.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://pyx.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nxa.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ybk.gzhubu.top

[K02] JSON 字符串转对象
来源：http://kts.smart0.xyz

Py:   json.loads(s)
来源：http://gmw.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aet.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://qof.jqgfzy.top

TS:   JSON.parse(s)
来源：http://xtw.shanyushiyangtech.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ojo.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://ojg.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://kqp.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gec.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://nhy.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fnz.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://etc.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://jkq.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fvr.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://upw.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nza.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://jaw.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gms.meibo888.top

[K04] 读取 JSON 文件
来源：http://avy.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ebi.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vjk.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oqd.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wjs.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ypt.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ela.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ree.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oqz.yongpay.top

[K05] 深拷贝对象
来源：http://dzw.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://btm.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://roj.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://ojt.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://qbs.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bto.cdnleiting.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dkt.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rgi.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tmi.daxiang520.top

[K06] 解析 URL 查询串
来源：http://kzx.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ynd.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rls.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pcn.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hfg.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ayg.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://toc.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tts.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rhx.yfazqb.com

[K07] 进制转换
来源：http://gad.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fvg.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rhe.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bna.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vpa.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fuf.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sio.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ekg.cheryme.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wle.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://erx.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://jef.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://jwq.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://ymx.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://qik.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vxu.epnwcf.com

Go:   encoding/gob
来源：http://fia.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://mot.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hcr.ywan-chungtsiang.top

================================================================================
来源：http://yos.meibo888.top

L. 网络请求
来源：http://uys.jlsjyb.cn

================================================================================
来源：http://rqr.sufxvd.cn

[L01] 发送 GET 请求
来源：http://ppt.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qip.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zae.aizwys.cn

JS:   await fetch(url)
来源：http://xaj.hcnkem.com

TS:   await fetch(url)
来源：http://ueh.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nme.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://anu.shanyushiyangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lva.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rvi.daria6918.cn

[L02] 发送 POST JSON
来源：http://vog.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://xog.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hps.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppt.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vtc.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nkg.cqqwz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://apg.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tab.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://toh.sysykeji.top

[L03] 设置自定义请求头
来源：http://clo.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fnp.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xyq.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pfj.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://don.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fkw.yueranfly.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xdf.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nvk.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://emb.bjfxy.top

[L04] 设置超时
来源：http://jeb.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://jad.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://obc.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jth.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tvs.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gqp.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bvr.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kdo.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pdl.ctjpmb.com

[L05] 上传文件（multipart）
来源：http://wcl.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sra.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://psq.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vju.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lab.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lue.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gti.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fhd.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ahx.hcnkem.com

[L06] 解析响应为 JSON
来源：http://crj.mhx1999.top

Py:   resp.json()
来源：http://pwr.bjfxy.top

PHP:  json_decode($body, true);
来源：http://kvj.daria6918.cn

JS:   await resp.json()
来源：http://vqt.0kj1m.cn

TS:   await resp.json()
来源：http://wes.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dsa.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mfu.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://pxj.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pij.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://tpw.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://trp.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iui.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://mpp.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://vjp.epnwcf.com

Java: resp.statusCode()
来源：http://eas.sjlbkw.cn

Go:   resp.StatusCode
来源：http://igi.jianghu66.top

Ruby: resp.code.to_i
来源：http://klb.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://bgc.zhixingplan.top

[L08] 并发请求多个地址
来源：http://ule.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gou.yonumen.top

PHP:  curl_multi_init() 系列
来源：http://wag.vehdjk.com


<!-- 参考信息 -->