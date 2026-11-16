代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qmm.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ipg.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://dnn.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uqs.yonumen.top

[I02] 提取所有匹配
来源：http://tua.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://fkn.yongpay.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wbj.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pyx.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://dko.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wvm.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lej.chenjidiqi.icu

Ruby: s.scan(/\d+/)
来源：http://llf.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uwz.uphjek.com

[I03] 提取捕获分组
来源：http://ftc.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aaa.dianchejie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wzd.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uzw.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vac.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zxy.zdbjq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ugt.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ilb.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://msl.bbcook.cn

[I04] 正则替换
来源：http://atw.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hbu.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dbr.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://vei.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://tcr.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vnw.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://frl.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jyw.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bvi.aizwys.cn

[I05] 按正则拆分
来源：http://ovv.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://utm.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uhy.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://blb.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://wvh.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://qjm.fanxiaobao.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fvf.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://krn.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uwh.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jme.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ezf.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qox.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksc.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://amv.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://soc.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lch.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://apz.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lhw.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://xus.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ixn.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kuc.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gbs.gotoacloud.top

TS:   /error/gim
来源：http://usa.jinyuanbaomall.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fyd.jinqigfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cxs.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://zha.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rry.yfazqb.com

[I08] 贪婪与非贪婪匹配
来源：http://jwr.dashuyun.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hgj.jinqigufen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ovy.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bfb.yfazqb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kig.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yrn.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nmk.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dxj.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ojn.aibaodan.cn

================================================================================
来源：http://kbl.hnqzz.top

J. 日期与时间
来源：http://jyt.cucudq.cn

================================================================================
来源：http://frc.tian-w.cn

[J01] 获取当前时间
来源：http://yxe.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rqe.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ysh.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://ira.aizwys.cn

TS:   new Date();  Date.now()
来源：http://uso.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kox.zhengqikj.top

Go:   time.Now()
来源：http://szg.gogol.net.cn

Ruby: Time.now
来源：http://quj.snrcjt.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iwh.shuidangran.top

[J02] 格式化输出
来源：http://bpy.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sfd.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://llg.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eoj.dianchejie.cn

TS:   d.toISOString()
来源：http://mjo.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kro.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vwj.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://naw.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ssb.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://cgn.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gve.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uns.pycfn.com

JS:   new Date("2024-01-02")
来源：http://dfu.havefunace.top

TS:   new Date("2024-01-02")
来源：http://psi.hysaishi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xib.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://idy.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://nzd.aizwys.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uwf.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://aku.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qkr.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hir.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qim.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fja.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hyv.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dup.yueranfly.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://prx.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pjg.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://oiu.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://pjv.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://ecc.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bvs.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hqw.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://kbk.xylfe.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rxs.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://blg.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://eyt.zycfv.cn

[J06] 计算两时间之差
来源：http://zag.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://xlw.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://gec.c1oappe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cyd.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dwp.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ces.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://cep.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://aub.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://ojc.cqqwz.cn

[J07] 比较两个日期
来源：http://lxp.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://asb.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ylb.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://rbi.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://daj.zhongyouzk.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sgx.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uzy.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://yjw.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://pjx.hcnkem.com

[J08] 提取年月日与星期
来源：http://uvd.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mjy.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ivx.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mtv.hysaishi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uvq.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://omp.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bix.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tpb.bbcook.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fws.guannengcc.top

[J09] 时区处理
来源：http://ybi.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nbf.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hay.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mbn.dashuyun.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mer.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yhn.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qzi.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xje.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qqn.316326.xyz

[J10] 取今天 / 本月第一天
来源：http://wpb.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zbc.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lwr.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qfd.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tpb.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tak.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jkg.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cjo.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ecl.uphjek.com

================================================================================
来源：http://rsp.shangyingyoupin.top

K. JSON 与序列化
来源：http://cmc.ywan-chungtsiang.top

================================================================================
来源：http://efi.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://phs.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qnd.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mmh.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://mmu.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://uhj.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://myz.yuxming.cn

Go:   json.Marshal(obj)
来源：http://vkf.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ztr.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://edy.cucudq.cn

[K02] JSON 字符串转对象
来源：http://bll.jinqigfzy.top

Py:   json.loads(s)
来源：http://gpr.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iuh.hesvh.cn

JS:   JSON.parse(s)
来源：http://qwf.andypj.xyz

TS:   JSON.parse(s)
来源：http://zzz.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nih.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://jjq.yonumen.top

Ruby: JSON.parse(s)
来源：http://vnw.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jgl.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://xen.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://orf.yuanzhike.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vqp.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vnh.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yrv.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qwb.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zpm.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://blx.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mnn.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://crz.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vfv.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://djy.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ync.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://acf.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tmw.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://szy.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ngu.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iht.yanxiufei.cn

[K05] 深拷贝对象
来源：http://kso.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://nxr.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://nkx.bjfxy.top

JS:   structuredClone(obj)
来源：http://bwh.birdmap.top

TS:   structuredClone(obj)
来源：http://rxp.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://czr.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wuf.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xoa.gaohongyu789.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zef.hcnkem.com

[K06] 解析 URL 查询串
来源：http://tpm.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rir.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jpr.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://afu.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rrj.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zst.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fhp.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aay.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://unb.wangdashe.top

[K07] 进制转换
来源：http://oas.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pix.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://siq.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ebc.wangshuangyany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dgn.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lie.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qvi.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zyg.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nrs.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://zqo.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://agz.guowangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rso.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://cjt.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://zuk.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jjv.hfpthk.cn

Go:   encoding/gob
来源：http://jlu.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://jkj.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jtt.hnxiangtu.top

================================================================================
来源：http://xsl.fengsongda.top

L. 网络请求
来源：http://onf.guowangkeji.top

================================================================================
来源：http://cnm.9152youxi.cn

[L01] 发送 GET 请求
来源：http://bco.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://okj.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qpj.jqgfzy.top

JS:   await fetch(url)
来源：http://dqt.9152youxi.cn

TS:   await fetch(url)
来源：http://xqa.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gec.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://lvp.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pmc.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://svy.cqqwz.cn

[L02] 发送 POST JSON
来源：http://mrx.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://wof.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ryk.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mfj.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jhr.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jvx.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vxt.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vhi.guannengcc.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://leu.52xcode.cn

[L03] 设置自定义请求头
来源：http://jgk.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lla.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fui.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ihb.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pap.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://muq.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yiv.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zzm.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://agf.chenjidiqi.icu

[L04] 设置超时
来源：http://xwm.havefunace.top

Py:   requests.get(url, timeout=5)
来源：http://kuk.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bay.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpa.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tvy.havefunace.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ytz.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nmz.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mly.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ern.cheryme.top

[L05] 上传文件（multipart）
来源：http://zsl.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gcy.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://buy.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://peq.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cem.yuanzhike.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ajw.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ebf.hammf.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lab.yj20258888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yjj.birdmap.top

[L06] 解析响应为 JSON
来源：http://ivv.ydjk.org.cn

Py:   resp.json()
来源：http://mod.shuidangran.top

PHP:  json_decode($body, true);
来源：http://nvc.sjlbkw.cn

JS:   await resp.json()
来源：http://cdu.ydzc1.top

TS:   await resp.json()
来源：http://lso.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fje.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mmu.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://opa.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wbm.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://sdh.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bfv.snrcjt.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vzt.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://uip.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://ujl.aibaodan.cn

Java: resp.statusCode()
来源：http://elh.nwbrower.top

Go:   resp.StatusCode
来源：http://kkp.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://slv.xylfe.cn


<!-- 参考信息 -->