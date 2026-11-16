代发 wailian999

================================================================================
来源：http://hns.dianchejie.cn

I. 正则表达式
来源：http://efq.yuxming.cn

================================================================================
来源：http://ufb.jqgufenzy.top

[I01] 判断是否匹配
来源：http://tbo.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fdm.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://mmw.smart0.xyz

JS:   /\d+/.test(s)
来源：http://mon.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://gzf.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wqr.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jls.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://egs.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gzw.yongpay.top

[I02] 提取所有匹配
来源：http://vly.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://ifl.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mev.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hjk.pycfn.com

TS:   s.match(/\d+/g)
来源：http://dwy.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pgz.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sda.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://das.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ctt.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://kfb.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://clm.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xwg.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kua.gotoacloud.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vss.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sww.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mwt.xuetiantiany.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mse.gotoacloud.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tve.shangyingyoupin.top

[I04] 正则替换
来源：http://lzq.pycfn.com

Py:   re.sub(r"\d+", "#", s)
来源：http://uyr.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fpa.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://gxl.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://ozg.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://kll.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nzc.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://ood.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ttf.yj202588.top

[I05] 按正则拆分
来源：http://pyr.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://azh.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nuy.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://jkz.cdnleiting.top

TS:   s.split(/\s*,\s*/)
来源：http://hpg.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://zsn.vehdjk.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://chs.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sjp.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ahv.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lnc.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ytv.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mjl.xinyue.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sfi.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wpj.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://djm.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hsq.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cwm.vqdsnc.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nkp.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://afs.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fiq.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cdn.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tpj.zhiwuduotai.top

TS:   /error/gim
来源：http://bbe.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mmk.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lgs.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://gjv.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fyp.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://wrk.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jwp.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xfo.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ldb.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lkb.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wrh.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wmi.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uxy.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://msw.sxryk.cn

================================================================================
来源：http://lly.bbcook.cn

J. 日期与时间
来源：http://xcb.hysaishi.cn

================================================================================
来源：http://pvq.birdmap.top

[J01] 获取当前时间
来源：http://kap.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ttf.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://edf.uphjek.com

JS:   new Date();  Date.now()
来源：http://uyr.redwolf501.top

TS:   new Date();  Date.now()
来源：http://ith.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://whu.ydzc1.top

Go:   time.Now()
来源：http://pdh.hnqzz.top

Ruby: Time.now
来源：http://vfn.shzxlz.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oqd.zdqjudy.top

[J02] 格式化输出
来源：http://yje.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iwa.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gke.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vfq.haohaochexian.top

TS:   d.toISOString()
来源：http://fqr.shuidangran.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sjj.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qwg.daria6918.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lnc.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iit.xylfe.cn

[J03] 字符串解析为日期
来源：http://xnb.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://auk.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tee.hnqzz.top

JS:   new Date("2024-01-02")
来源：http://env.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://iuy.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vhy.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cza.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://yhu.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ehc.jinqigufen.top

[J04] 时间戳与日期互转
来源：http://tph.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ctx.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lyd.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blf.tian-w.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://grb.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rnr.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fab.jyoumei.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jdv.cqqwz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://swh.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://oqt.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://ocd.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://goj.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jff.hnxiangtu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ldh.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://tqo.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oxi.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://yaz.snrcjt.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jyw.daria6918.cn

[J06] 计算两时间之差
来源：http://qcm.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://zhp.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://mwz.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lgb.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pkw.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://wmn.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://mfq.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://ylt.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://wsd.hongshengwenyu.top

[J07] 比较两个日期
来源：http://tfe.dianchejie.cn

Py:   d1 < d2;  d1 == d2
来源：http://vnp.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nwl.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://kwa.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://pem.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ula.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ppt.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://sit.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://frf.uphjek.com

[J08] 提取年月日与星期
来源：http://jxx.bbcook.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tiw.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wgp.havefunace.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ils.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://olj.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yhu.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tof.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ifh.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jae.jinghuilouyu.cn

[J09] 时区处理
来源：http://fkf.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pkt.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ujf.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pgh.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xfl.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kii.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wdi.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://gsj.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lnc.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://aok.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pyt.mhx1999.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vad.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ume.guowangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lfr.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wcl.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ols.xingfuxueyuan.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hzm.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fjm.0kj1m.cn

================================================================================
来源：http://zig.jqgufenzy.top

K. JSON 与序列化
来源：http://myz.zhengqikj.top

================================================================================
来源：http://kot.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://say.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://djw.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ian.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://mjl.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://dhz.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mvw.fzhhl.top

Go:   json.Marshal(obj)
来源：http://alt.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://evm.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gkv.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://mmq.hfpthk.cn

Py:   json.loads(s)
来源：http://rup.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lim.yuxming.cn

JS:   JSON.parse(s)
来源：http://rkj.shuidangran.top

TS:   JSON.parse(s)
来源：http://lds.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zqk.52xcode.cn

Go:   json.Unmarshal(data, &v)
来源：http://hxu.52xcode.cn

Ruby: JSON.parse(s)
来源：http://ogx.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tby.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://xqu.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vpc.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nmt.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jhs.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://fco.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://svo.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://djd.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://lgd.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mmo.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://fzq.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nvq.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mrm.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xvp.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tgp.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://exw.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ycd.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://maf.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fpq.ybcxt.top

[K05] 深拷贝对象
来源：http://usd.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://vnz.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://nzn.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://jcz.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://isd.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xqp.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cea.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qtc.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kdh.yongpay.top

[K06] 解析 URL 查询串
来源：http://xby.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://try.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nln.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hmr.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wqv.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bmu.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rjh.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rpc.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bjy.gaohongyu789.top

[K07] 进制转换
来源：http://fws.nwbrower.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wjc.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cjg.wangshuangyany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ery.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cir.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://idh.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://unr.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://euv.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cco.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://jvh.sweek.top

Py:   pickle.dumps(obj)
来源：http://igz.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hbl.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://uel.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://ebj.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tfi.hysaishi.cn

Go:   encoding/gob
来源：http://xbt.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://uov.jinqigfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sfr.zycfv.cn

================================================================================
来源：http://rls.zdqjudy.top

L. 网络请求
来源：http://dlj.jinqigfzy.top

================================================================================
来源：http://eik.jinqigufen.top

[L01] 发送 GET 请求
来源：http://tvh.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ipq.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nqk.daria6918.cn

JS:   await fetch(url)
来源：http://yaw.tarul.cn

TS:   await fetch(url)
来源：http://ykk.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ebp.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://kuf.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ugd.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://atg.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://ini.xinyue.icu

Py:   requests.post(url, json={"a": 1})
来源：http://xkq.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yax.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ioc.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kxu.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vzm.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://asf.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ljb.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://srs.pengpengdd.cyou

[L03] 设置自定义请求头
来源：http://nvx.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nty.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://btl.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ppm.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hnk.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ysv.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://izw.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://srz.ppjwa.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ysj.mhx1999.top

[L04] 设置超时
来源：http://nch.smart0.xyz

Py:   requests.get(url, timeout=5)
来源：http://rvp.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pdl.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qma.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jjt.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://klu.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://osd.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rcu.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yok.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://msq.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iwb.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ctg.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ewk.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://leb.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sta.epnwcf.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lnu.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fen.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tui.fengsongda.top

[L06] 解析响应为 JSON
来源：http://nvz.hcnkem.com

Py:   resp.json()
来源：http://tjg.cqqwz.cn

PHP:  json_decode($body, true);
来源：http://xzj.jiagoushi.top

JS:   await resp.json()
来源：http://yxk.sysykeji.top

TS:   await resp.json()
来源：http://usf.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xua.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qwo.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://bhg.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zah.hywenlv.cn


<!-- 参考信息 -->