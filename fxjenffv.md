代发 wailian999

[I02] 提取所有匹配
来源：http://puy.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://mqk.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://svb.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://muh.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://syf.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nku.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cea.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://skc.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ays.zycfv.cn

[I03] 提取捕获分组
来源：http://ucp.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jcw.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ptp.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fwg.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hbj.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lea.yuanzhike.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://trj.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tfp.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zdy.316326.xyz

[I04] 正则替换
来源：http://xnh.gotoacloud.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bsc.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ytt.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kyv.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://gfi.tanke756.top

Java: s.replaceAll("\\d+", "#")
来源：http://znn.52xcode.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ayc.iojbl.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://npc.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nfk.zhiwuduotai.top

[I05] 按正则拆分
来源：http://seb.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xjq.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yyq.bjfxy.top

JS:   s.split(/\s*,\s*/)
来源：http://sqv.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://nuh.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://uiq.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nlv.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://dpg.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cni.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qqw.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://btn.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rhd.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ubz.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nit.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pju.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vlr.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ddf.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xju.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://lnb.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xlh.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rac.bjfxy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ese.chenjidiqi.icu

TS:   /error/gim
来源：http://rmp.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bnv.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dxq.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://ppa.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rrv.xuanzx.com

[I08] 贪婪与非贪婪匹配
来源：http://wcz.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ldo.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://elz.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xzb.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ugo.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gja.yj202588.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wha.hfpthk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xlb.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pho.xziqi.cn

================================================================================
来源：http://jfy.meibo888.top

J. 日期与时间
来源：http://iir.haohaochexian.top

================================================================================
来源：http://naz.snrcjt.cn

[J01] 获取当前时间
来源：http://dgo.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rfa.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://evu.bbcook.cn

JS:   new Date();  Date.now()
来源：http://rum.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://nfm.dianchejie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://puf.yj20258.top

Go:   time.Now()
来源：http://alw.nanxuanxn.top

Ruby: Time.now
来源：http://sqx.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lvj.tanke756.top

[J02] 格式化输出
来源：http://mgk.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://otj.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hno.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iqq.hongshengwenyu.top

TS:   d.toISOString()
来源：http://nrt.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fin.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ncd.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://npt.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://utv.yj20258888.top

[J03] 字符串解析为日期
来源：http://eae.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dtt.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vas.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://jjx.fengsongda.top

TS:   new Date("2024-01-02")
来源：http://zjl.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://tes.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eqf.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://adj.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ldk.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://zvr.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mby.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kcd.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tvs.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://jnu.pengpengdd.cyou

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://liu.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lfk.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://waw.yuxming.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://due.cqqwz.cn

[J05] 时间加减（加 7 天）
来源：http://wrn.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://mlp.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zta.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hcl.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://swj.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://pjd.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iih.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://xrq.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://npv.ppjwa.cn

[J06] 计算两时间之差
来源：http://cmq.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://dcp.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://onk.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://osq.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iem.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wxs.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://unh.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://anc.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://wzd.sweek.top

[J07] 比较两个日期
来源：http://xmd.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://mqt.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gve.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://cvh.jiagoushi.top

TS:   d1.getTime() < d2.getTime()
来源：http://dkx.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tez.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uad.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://jqy.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://tww.snrcjt.cn

[J08] 提取年月日与星期
来源：http://opn.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rpc.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gsc.hongshengwenyu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pve.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eoy.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qzy.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jjw.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ckj.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ajr.yj20258.top

[J09] 时区处理
来源：http://ecz.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oum.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ugq.jqgfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cly.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mqn.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gbr.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nfp.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://dgi.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hxa.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://uxp.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nhu.kuanghao11.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vdm.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wjz.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kvc.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uly.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vwl.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gau.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hpy.sxryk.cn

================================================================================
来源：http://iuf.guannengcc.top

K. JSON 与序列化
来源：http://ypy.xziqi.cn

================================================================================
来源：http://fgu.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://kex.ydjk.org.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cbo.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qth.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://nuw.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://epy.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sti.yuxming.cn

Go:   json.Marshal(obj)
来源：http://mra.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://hjo.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ghw.vehdjk.com

[K02] JSON 字符串转对象
来源：http://dpm.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://aos.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zpr.cdnleiting.top

JS:   JSON.parse(s)
来源：http://zir.epnwcf.com

TS:   JSON.parse(s)
来源：http://dkr.guannengcc.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lkl.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://ckv.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://tgp.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bzy.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://gyx.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://snj.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tma.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wgb.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://twt.xziqi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oaq.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uwu.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tkp.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rbh.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://wtp.yuxming.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://faj.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hou.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rpq.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zmp.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wgg.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ewu.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vua.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kem.yuxming.cn

[K05] 深拷贝对象
来源：http://ujv.haohaochexian.top

Py:   copy.deepcopy(obj)
来源：http://mif.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://cmb.pycfn.com

JS:   structuredClone(obj)
来源：http://uoi.yuanzhike.top

TS:   structuredClone(obj)
来源：http://eop.ywan-chungtsiang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mkz.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://spc.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sef.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://zah.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://mfx.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yft.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ozs.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kka.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wgm.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rrq.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dsl.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cqh.ydzc1.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kzw.fengsongda.top

[K07] 进制转换
来源：http://bzg.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://arh.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://joc.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yvv.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wrv.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jcy.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lbr.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uya.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://irl.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://vls.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://dez.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://diu.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://gwg.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://lyz.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ejx.nanxinkj.top

Go:   encoding/gob
来源：http://jaw.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://suq.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qnj.zhaomingkeji.xyz

================================================================================
来源：http://uaf.ybcxt.top

L. 网络请求
来源：http://zdp.havefunace.top

================================================================================
来源：http://wnr.guowangkeji.top

[L01] 发送 GET 请求
来源：http://jui.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xjm.tanke756.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vjs.jinqigfzy.top

JS:   await fetch(url)
来源：http://enb.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://rmn.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oqb.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://nya.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://zmt.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iax.hcnkem.com

[L02] 发送 POST JSON
来源：http://fwj.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://ijr.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ztt.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gat.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hqh.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://obq.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yqe.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oza.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gfc.cashguo.top

[L03] 设置自定义请求头
来源：http://wne.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wel.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kna.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://szs.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vuy.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lhj.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zot.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xqg.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uwe.xylfe.cn

[L04] 设置超时
来源：http://jnm.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://qra.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zbh.sweek.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sec.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mgt.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qdy.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tye.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://irj.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vdp.xuanzx.com

[L05] 上传文件（multipart）
来源：http://odo.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zqx.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yez.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ysf.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://msc.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iob.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rmv.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mhq.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xck.bjfxy.top

[L06] 解析响应为 JSON
来源：http://upd.shuidangran.top

Py:   resp.json()
来源：http://xjm.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://qzo.gogol.net.cn

JS:   await resp.json()
来源：http://cbs.jinqigfzy.top

TS:   await resp.json()
来源：http://tum.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://spg.yongpay.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zpe.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://jst.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kkx.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://jxs.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ots.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dby.316326.xyz

JS:   resp.ok;  resp.status
来源：http://iwi.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://pyn.quarkkingdee.top

Java: resp.statusCode()
来源：http://mbv.daxiang520.top

Go:   resp.StatusCode
来源：http://lxm.sweek.top

Ruby: resp.code.to_i
来源：http://kpr.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://imu.bjfxy.top

[L08] 并发请求多个地址
来源：http://pbo.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ook.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://rxy.sufxvd.cn


<!-- 参考信息 -->