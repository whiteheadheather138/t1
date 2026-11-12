代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hmi.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uuf.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rvb.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://igg.xuetiantiany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ksc.sweek.top

Go:   defer f.Close()
来源：http://llh.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://swf.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cdb.ybcxt.top

================================================================================
来源：http://bcg.yj20258.top

I. 正则表达式
来源：http://gyu.jiagoushi.top

================================================================================
来源：http://nav.fktsv.cn

[I01] 判断是否匹配
来源：http://ipz.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://btg.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://xyf.shuidangran.top

JS:   /\d+/.test(s)
来源：http://cns.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://zjo.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://odc.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hdm.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://mqd.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lrc.xuanzx.com

[I02] 提取所有匹配
来源：http://wxb.52xcode.cn

Py:   re.findall(r"\d+", s)
来源：http://wtx.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://une.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yvj.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://dpe.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mfu.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dwn.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://owh.tian-w.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cpv.nanxinkj.top

[I03] 提取捕获分组
来源：http://kfk.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kwu.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wuz.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fkj.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wnf.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gcy.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xow.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dao.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ywk.0kj1m.cn

[I04] 正则替换
来源：http://jmn.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://thh.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yid.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eaw.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://xax.tarul.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ubf.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uah.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jsc.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iby.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://gwb.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://aap.iojbl.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ise.yvedp.cn

JS:   s.split(/\s*,\s*/)
来源：http://oxo.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://ufa.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://vcy.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zsg.hcnkem.com

Ruby: s.split(/\s*,\s*/)
来源：http://jhh.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gdt.xinyue.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dgd.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bsd.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://din.hfpthk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://opk.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jhv.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xta.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xta.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qab.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ztz.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://rtx.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lhs.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lvt.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zyj.shanyushiyangtech.top

TS:   /error/gim
来源：http://avd.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vpc.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uvb.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://wxo.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yvz.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://bnu.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mas.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ndt.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ycs.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dgg.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vzy.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cxc.gzhubu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gyw.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ghn.316326.xyz

================================================================================
来源：http://kfz.zycfv.cn

J. 日期与时间
来源：http://axi.daria6918.cn

================================================================================
来源：http://ozh.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://xub.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pju.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://haz.hywenlv.cn

JS:   new Date();  Date.now()
来源：http://guc.sxryk.cn

TS:   new Date();  Date.now()
来源：http://xen.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://uvq.dianchejie.cn

Go:   time.Now()
来源：http://xte.daria6918.cn

Ruby: Time.now
来源：http://ydc.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eim.fehbvm.com

[J02] 格式化输出
来源：http://yjt.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ylx.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tkk.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qqw.cucudq.cn

TS:   d.toISOString()
来源：http://gsm.hfpthk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yek.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hou.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hec.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rkw.daria6918.cn

[J03] 字符串解析为日期
来源：http://xlv.zycfv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xlp.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wga.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://tfq.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://keu.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://tkv.pycfn.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bfc.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://qjc.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lag.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://cut.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xik.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hsi.yanxiufei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wxp.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://qxa.jiagoushi.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bzf.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jty.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mzb.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xdi.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://zqk.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://uih.ivvv.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gii.0kj1m.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ble.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vck.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ccw.jqgfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wwc.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://dqm.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://blz.shuidangran.top

[J06] 计算两时间之差
来源：http://vqy.yj20258.top

Py:   (end - start).total_seconds()
来源：http://bzo.svipenyu.cn

PHP:  $end->diff($start)->days;
来源：http://lyi.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bsq.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nne.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://emg.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://ifx.ywan-chungtsiang.top

Ruby: end - start                 # 返回秒数
来源：http://mot.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://bfh.redwolf501.top

[J07] 比较两个日期
来源：http://tfk.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://pgj.nanxuanxn.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fit.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://grl.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xjk.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yng.chenzaomai.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ddh.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dut.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://now.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://azb.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://atq.cucudq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jma.nanxuanxn.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cdp.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wey.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wry.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sor.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fen.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mnz.yueranfly.top

[J09] 时区处理
来源：http://mtj.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qjp.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://umw.vehdjk.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aec.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qjx.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uxz.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ast.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bam.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pxr.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://rqp.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://egw.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hqu.sufxvd.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xqr.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cis.hnxiangtu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://buu.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mpm.hfpthk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wlu.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tpk.yuxming.cn

================================================================================
来源：http://iwm.haohaochexian.top

K. JSON 与序列化
来源：http://nmz.xuetiantiany.cn

================================================================================
来源：http://kap.shangyingyoupin.top

[K01] 对象转 JSON 字符串
来源：http://hdm.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pbf.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bsj.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://zmb.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://zmd.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wgr.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://zcr.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://iid.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://enp.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://fdx.zhoulong.xyz

Py:   json.loads(s)
来源：http://pay.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mez.jyoumei.cn

JS:   JSON.parse(s)
来源：http://dwz.pycfn.com

TS:   JSON.parse(s)
来源：http://ypr.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rnj.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://jlk.yfazqb.com

Ruby: JSON.parse(s)
来源：http://uqx.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dei.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://cfy.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mup.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://keg.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://qeg.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mqy.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://thr.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qef.bjfxy.top

Ruby: JSON.pretty_generate(obj)
来源：http://jof.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qkc.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://bed.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fsd.hywenlv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bcv.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mfr.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://skw.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gqd.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wim.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kyv.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bkb.chenzaomai.com

[K05] 深拷贝对象
来源：http://wcu.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://hyw.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://kdx.dianchejie.cn

JS:   structuredClone(obj)
来源：http://vpi.316326.xyz

TS:   structuredClone(obj)
来源：http://ufe.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wup.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yjs.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sak.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pzg.pycfn.com

[K06] 解析 URL 查询串
来源：http://dhu.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cff.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qbf.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tzv.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jwy.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://crr.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://joy.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://euw.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lvk.sweek.top

[K07] 进制转换
来源：http://kii.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yif.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kbh.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rph.dashuyun.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rue.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ljo.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sgv.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jud.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://duf.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://svr.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://pgr.gotoacloud.top

PHP:  serialize($obj);  unserialize($s);
来源：http://moa.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://rnj.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://dbu.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qyo.zhongyouzk.top

Go:   encoding/gob
来源：http://jcs.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://obk.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hqx.ehwqpu.com

================================================================================
来源：http://npf.ybcxt.top

L. 网络请求
来源：http://ufm.zhongyouzk.top

================================================================================
来源：http://ced.jiagoushi.top

[L01] 发送 GET 请求
来源：http://xmz.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kpu.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cfp.jyoumei.cn

JS:   await fetch(url)
来源：http://vix.fengsongda.top

TS:   await fetch(url)
来源：http://pxc.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mat.epnwcf.com

Go:   resp, err := http.Get(url)
来源：http://qqy.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lkg.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tdo.bjfxy.top

[L02] 发送 POST JSON
来源：http://xkt.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://wgg.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cuq.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yvd.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yhj.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nad.shanyushiyangtech.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ocm.sysykeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kxt.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dnp.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://rzd.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oit.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tnt.xinyue.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://elz.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eye.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://elr.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pzu.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iaz.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qry.smart0.xyz

[L04] 设置超时
来源：http://nli.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://xsk.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://utr.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nty.nanxuanxn.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dbt.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mgd.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kjm.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://agl.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ixe.fehbvm.com

[L05] 上传文件（multipart）
来源：http://vfe.chenjidiqi.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://elj.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cny.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vnh.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pmh.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nlw.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cyw.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cfq.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ego.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://lrp.hywenlv.cn


<!-- 参考信息 -->