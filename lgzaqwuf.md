代发 wailian999

[I02] 提取所有匹配
来源：http://kxk.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://dlb.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gmr.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jog.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://dcj.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wyi.hnqzz.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bby.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://gxn.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ejv.birdmap.top

[I03] 提取捕获分组
来源：http://ctq.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xev.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hpn.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rog.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://skw.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://giv.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://agb.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kca.gaohongyu789.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vdh.zhijiandao.cn

[I04] 正则替换
来源：http://cfw.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hjx.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aqq.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://fgo.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oet.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://iif.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qsd.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qsa.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mww.zhongyouzk.top

[I05] 按正则拆分
来源：http://chp.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zgy.redwolf501.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nvx.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://tql.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://hzj.sjlbkw.cn

Java: s.split("\\s*,\\s*")
来源：http://aub.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vdc.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jle.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lvz.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sbq.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wbo.yj20258.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iro.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hoy.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zoa.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vlv.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mqw.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xym.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fsw.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://hma.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mso.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nnj.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cft.yueranfly.top

TS:   /error/gim
来源：http://xmz.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ijk.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qss.ivvv.top

Ruby: s.scan(/error/i)
来源：http://keu.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://weo.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://giv.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fvl.pengpengdd.cyou

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dzl.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ylr.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bgh.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kdg.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nou.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xnn.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gbo.fehbvm.com

================================================================================
来源：http://xnt.sjlbkw.cn

J. 日期与时间
来源：http://xgr.0kj1m.cn

================================================================================
来源：http://zty.feifeiyinyue.top

[J01] 获取当前时间
来源：http://lsb.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ffa.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tlh.yfazqb.com

JS:   new Date();  Date.now()
来源：http://wfg.yj202588.top

TS:   new Date();  Date.now()
来源：http://oin.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wmj.hnxiangtu.top

Go:   time.Now()
来源：http://bgx.yj20258.top

Ruby: Time.now
来源：http://ycp.tian-w.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yht.mhx1999.top

[J02] 格式化输出
来源：http://iwz.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzy.jianghu66.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qxb.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ecx.epnwcf.com

TS:   d.toISOString()
来源：http://ziv.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qvb.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bgi.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xwm.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ekk.yongpay.top

[J03] 字符串解析为日期
来源：http://wlh.svipenyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lqt.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pmw.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://mdk.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://mxq.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vza.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mlo.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://rrg.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cbu.ydjk.org.cn

[J04] 时间戳与日期互转
来源：http://olq.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://riu.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tcy.feifeiyinyue.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jmi.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://agt.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qyo.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cgy.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eer.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ycy.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://tvo.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://han.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xjj.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://evh.tanke756.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xtt.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://fwa.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mio.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://chs.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hyk.tarul.cn

[J06] 计算两时间之差
来源：http://fth.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://uam.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://hjv.gzhubu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lma.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://osv.zhijiandao.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xap.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://aer.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://lxn.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://wrv.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://kyy.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://mqa.hywenlv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tvt.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://hpi.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://eyw.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tig.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hgj.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://glr.hywenlv.cn

C#:   d1 < d2;  d1 == d2
来源：http://vgu.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://pgy.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tst.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zal.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://npr.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://prz.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xit.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://arr.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zhw.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fuv.yj202588.top

[J09] 时区处理
来源：http://ctl.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nbt.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hvz.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sek.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uiw.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qsj.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://asj.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://wnc.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rrc.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://dvh.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bak.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kvp.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nfx.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ikm.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://igu.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://owe.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://opf.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kod.yuxming.cn

================================================================================
来源：http://zwu.chenjidiqi.icu

K. JSON 与序列化
来源：http://tdf.cashguo.top

================================================================================
来源：http://jkj.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://ttr.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fvp.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oqm.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://qsz.yongpay.top

TS:   JSON.stringify(obj)
来源：http://lqg.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wnt.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://xpe.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://mcg.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vpb.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://zbl.yangfankeji.com

Py:   json.loads(s)
来源：http://tvx.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pvm.meibo888.top

JS:   JSON.parse(s)
来源：http://swd.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://lvc.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dsa.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://bsc.hammf.cn

Ruby: JSON.parse(s)
来源：http://cvx.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nxh.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://oos.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://soc.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iyv.wangdashe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hcx.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ghu.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tqz.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mhe.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dof.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uxa.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://vrp.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tmp.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://siv.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fzp.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rkr.bjfxy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qky.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bmq.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://opu.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tsl.gotoacloud.top

[K05] 深拷贝对象
来源：http://ugs.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://tcb.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://iyl.daria6918.cn

JS:   structuredClone(obj)
来源：http://bkg.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://quw.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wrp.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zrs.hnqzz.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://awb.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zhk.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://olt.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qnq.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nov.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mhx.snrcjt.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eep.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lhy.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://drh.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qza.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ian.hcnkem.com

[K07] 进制转换
来源：http://bff.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wpw.aibaodan.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://asw.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://avj.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pux.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://icu.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wtt.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xdb.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oat.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://eay.ydjk.org.cn

Py:   pickle.dumps(obj)
来源：http://cnv.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://uwi.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://vlp.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://kos.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://evc.shuidangran.top

Go:   encoding/gob
来源：http://moe.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://jry.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bfi.feifeiyinyue.top

================================================================================
来源：http://ggd.chenzaomai.com

L. 网络请求
来源：http://wqv.zhijiandao.cn

================================================================================
来源：http://fyu.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://sqe.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tor.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ziu.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://oci.fzhhl.top

TS:   await fetch(url)
来源：http://dfx.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bgx.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://mdc.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xre.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vwo.tanke756.top

[L02] 发送 POST JSON
来源：http://qwl.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mhs.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nka.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://neg.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ixo.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zcj.tian-w.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xdz.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gpe.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://afi.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://soq.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lxq.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lrg.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://haw.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://clu.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zln.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ekf.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vcf.zdbjq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gvk.9152youxi.cn

[L04] 设置超时
来源：http://unh.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://ccv.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hkt.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hcn.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kcq.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wqu.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lhe.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tpv.zhaomingkeji.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hct.iojbl.cn

[L05] 上传文件（multipart）
来源：http://god.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vvd.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zuy.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ekb.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gpq.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dou.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ffa.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jmq.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dmv.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://irg.jyoumei.cn

Py:   resp.json()
来源：http://zkx.zhengqikj.top

PHP:  json_decode($body, true);
来源：http://fhv.tian-w.cn

JS:   await resp.json()
来源：http://svs.xinyue.icu

TS:   await resp.json()
来源：http://fws.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qqa.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kkh.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://trw.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pny.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://yun.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pun.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://umg.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://frr.sufxvd.cn

TS:   resp.ok;  resp.status
来源：http://hfv.birdmap.top

Java: resp.statusCode()
来源：http://ynx.fengsongda.top

Go:   resp.StatusCode
来源：http://nrc.gzhubu.top

Ruby: resp.code.to_i
来源：http://jnp.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://hki.birdmap.top

[L08] 并发请求多个地址
来源：http://owc.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ebt.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://bmv.gotoacloud.top


<!-- 参考信息 -->