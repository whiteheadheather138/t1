代发 wailian999

[I02] 提取所有匹配
来源：http://kjy.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://lgb.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ztu.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tsz.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://tvs.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qgw.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nge.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://qfo.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wvr.yuxming.cn

[I03] 提取捕获分组
来源：http://cfm.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gow.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gmn.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zch.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vxj.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zcw.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cgd.havefunace.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rhy.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ytk.cdnleiting.top

[I04] 正则替换
来源：http://kpa.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zog.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lnc.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dya.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mci.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://mru.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ygr.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://pup.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bft.epnwcf.com

[I05] 按正则拆分
来源：http://myp.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hbi.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nnv.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://pnr.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://xme.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://vzh.c1oappe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hsi.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://drx.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://htn.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rkx.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wbn.xuetiantiany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gfv.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dqm.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xay.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fbd.zhongyouzk.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zrg.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yko.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wtp.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://fvp.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lnt.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bbz.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://muq.yj20258888.top

TS:   /error/gim
来源：http://kda.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sly.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ewt.dianchejie.cn

Ruby: s.scan(/error/i)
来源：http://lrd.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hel.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://toj.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://urt.cdnleiting.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ntq.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ckr.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vjn.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hzd.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nyx.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qyb.sjlbkw.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nel.yongpay.top

================================================================================
来源：http://rcm.tian-w.cn

J. 日期与时间
来源：http://rrx.iojbl.cn

================================================================================
来源：http://aym.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://ljm.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://dlz.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://njc.zycfv.cn

JS:   new Date();  Date.now()
来源：http://dlx.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://ltl.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://img.svipenyu.cn

Go:   time.Now()
来源：http://ann.yvedp.cn

Ruby: Time.now
来源：http://hql.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ufs.hesvh.cn

[J02] 格式化输出
来源：http://ptq.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rlt.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qmq.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wfc.sufxvd.cn

TS:   d.toISOString()
来源：http://tvp.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tfn.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://syk.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xxf.yanxiufei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zji.cucudq.cn

[J03] 字符串解析为日期
来源：http://qyn.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lle.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vwf.yj202588.top

JS:   new Date("2024-01-02")
来源：http://utx.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://xvk.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://ehx.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jjx.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://jqu.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sud.shuidangran.top

[J04] 时间戳与日期互转
来源：http://bbk.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mqa.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baj.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://klg.yj20258888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sbq.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yme.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yxy.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cns.9152youxi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://umd.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://qxn.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://mce.jinqigufen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ybs.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpd.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xjm.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://sit.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hgo.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://aix.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://ehe.cheryme.top

[J06] 计算两时间之差
来源：http://ewt.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://pkx.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://ati.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ebx.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bli.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://inj.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://qne.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://rec.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://pgo.hnqzz.top

[J07] 比较两个日期
来源：http://dsi.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://qyj.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uks.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rjo.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://scf.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hhu.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://imj.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://szl.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://jhc.andypj.xyz

[J08] 提取年月日与星期
来源：http://kgz.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tnp.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rfd.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://brp.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jky.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://njf.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fmv.ctjpmb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fyn.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eji.feifeiyinyue.top

[J09] 时区处理
来源：http://rre.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zbi.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gbp.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://psx.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oiw.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tvb.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tnp.yj20258.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qvt.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rmc.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://ejt.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://joa.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://evh.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hqp.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qqv.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tyu.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mnc.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dfw.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ueh.sysykeji.top

================================================================================
来源：http://vmr.svipenyu.cn

K. JSON 与序列化
来源：http://ybh.zhixingplan.top

================================================================================
来源：http://sec.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://acu.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ayq.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oqx.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://cpq.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://ncd.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xit.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://yxe.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://bxn.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dkb.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://ffv.fzhhl.top

Py:   json.loads(s)
来源：http://kqp.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://saj.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://jpp.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://ejn.bbcook.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hqo.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://cao.yj20258888.top

Ruby: JSON.parse(s)
来源：http://siq.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zrk.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://kkj.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rou.316326.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mbu.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dwr.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://khc.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ytm.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cjt.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://kfp.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eyb.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://pck.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ygk.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://die.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tlv.ivvv.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wcs.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jjp.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pmp.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nbo.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wwt.birdmap.top

[K05] 深拷贝对象
来源：http://bgb.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://lrc.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://fle.yueranfly.top

JS:   structuredClone(obj)
来源：http://sjo.daxiang520.top

TS:   structuredClone(obj)
来源：http://kgb.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://efl.zhixingplan.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vah.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sih.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sva.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://mku.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xou.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gvh.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vpo.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jyg.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gxu.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://qvg.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ceo.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://loj.yfazqb.com

[K07] 进制转换
来源：http://pjr.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fse.snrcjt.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://azt.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://obi.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qji.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hxu.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jdf.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://com.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kfj.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://vlv.yonumen.top

Py:   pickle.dumps(obj)
来源：http://edh.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cxl.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://tcz.sweek.top

TS:   v8.serialize(obj)        // Node
来源：http://gxf.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pgz.pengpengdd.cyou

Go:   encoding/gob
来源：http://vha.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://btl.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://otz.yj20258.top

================================================================================
来源：http://bwm.xziqi.cn

L. 网络请求
来源：http://xnf.feifeiyinyue.top

================================================================================
来源：http://rue.jlsjyb.cn

[L01] 发送 GET 请求
来源：http://iqq.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ouc.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://edv.yongpay.top

JS:   await fetch(url)
来源：http://ecp.jinqigufen.top

TS:   await fetch(url)
来源：http://lau.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rwk.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://ahc.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dpi.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://avb.hywenlv.cn

[L02] 发送 POST JSON
来源：http://svb.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://rak.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://puh.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tkh.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rfy.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tkj.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mmi.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lsh.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iap.tanke756.top

[L03] 设置自定义请求头
来源：http://wlq.svipenyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qtj.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tiv.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ump.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://krl.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://reo.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ppl.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iqw.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://auj.shanyushiyangkeji.top

[L04] 设置超时
来源：http://qvh.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://mkk.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vdm.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://act.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hqd.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rfl.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tnr.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cne.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://txq.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://xef.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://akh.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ctm.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zsl.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hdv.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://asw.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://obx.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sja.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rib.cheryme.top

[L06] 解析响应为 JSON
来源：http://ztc.ybcxt.top

Py:   resp.json()
来源：http://jew.tarul.cn

PHP:  json_decode($body, true);
来源：http://zni.xylfe.cn

JS:   await resp.json()
来源：http://ddy.tian-w.cn

TS:   await resp.json()
来源：http://ebm.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mfe.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vqc.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://zkc.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nlf.yj20258.top

[L07] 处理 HTTP 状态码
来源：http://qno.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gjx.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mcj.tanke756.top

JS:   resp.ok;  resp.status
来源：http://tjo.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://vjw.sweek.top

Java: resp.statusCode()
来源：http://azj.zycfv.cn

Go:   resp.StatusCode
来源：http://lqq.chenlongwang.top

Ruby: resp.code.to_i
来源：http://ule.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://vij.tian-w.cn

[L08] 并发请求多个地址
来源：http://lms.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qfo.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://dgg.tanke756.top


<!-- 参考信息 -->