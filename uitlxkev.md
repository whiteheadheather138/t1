代发 wailian999

================================================================================
来源：http://lrk.feifeiyinyue.top

I. 正则表达式
来源：http://rra.aibaodan.cn

================================================================================
来源：http://zgx.meibo888.top

[I01] 判断是否匹配
来源：http://mwu.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://feg.xinyue.icu

PHP:  preg_match('/\d+/', $s);
来源：http://lpy.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://uep.fzhhl.top

TS:   /\d+/.test(s)
来源：http://wha.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ljw.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dei.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://gbn.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tdk.jiagoushi.top

[I02] 提取所有匹配
来源：http://bgq.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://idb.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pku.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mab.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://vrv.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kbn.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nqq.xylfe.cn

Ruby: s.scan(/\d+/)
来源：http://cwd.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kqs.yanxiufei.cn

[I03] 提取捕获分组
来源：http://xla.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rik.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pxp.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pip.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mwd.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hcp.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mxg.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gie.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ipd.guannengcc.top

[I04] 正则替换
来源：http://kgj.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://hfm.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ncg.hnqzz.top

JS:   s.replace(/\d+/g, "#")
来源：http://ohr.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://oxy.tian-w.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cpz.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tib.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hqe.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mfy.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://xul.zdqjudy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://aft.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gyj.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://iwj.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://wsv.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://bpu.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://you.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://lci.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qoe.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jge.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dmp.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rws.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cno.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xeu.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cgn.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vac.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://raz.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bwy.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://nwf.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ysv.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uek.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wug.316326.xyz

TS:   /error/gim
来源：http://bxk.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lxp.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pmx.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://mcd.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rcy.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://yat.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qzq.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eoi.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vrs.yuanzhike.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xoh.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://czj.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fik.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ioy.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oss.xuetiantiany.cn

================================================================================
来源：http://hry.hnqzz.top

J. 日期与时间
来源：http://myt.ybcxt.top

================================================================================
来源：http://sek.yfazqb.com

[J01] 获取当前时间
来源：http://tzd.aibaodan.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bft.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rjz.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://xnk.pycfn.com

TS:   new Date();  Date.now()
来源：http://ucm.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mqn.epnwcf.com

Go:   time.Now()
来源：http://mic.hnxiangtu.top

Ruby: Time.now
来源：http://ohq.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hhc.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://vkb.zdqjudy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cfi.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qqy.ybcxt.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ooi.ybcxt.top

TS:   d.toISOString()
来源：http://uxj.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fes.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pel.jinqigfzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://idl.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zyp.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://ihb.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dgp.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bdc.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://akt.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://cpp.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gru.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://umg.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://trh.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zfv.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://znj.c1oappe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uoy.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xjz.ehwqpu.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eej.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vzk.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jui.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hsh.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fxv.epnwcf.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cwu.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://wgq.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://hfz.dianchejie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zvt.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sfg.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vgu.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://ndi.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ivo.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://nvf.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gzz.ehwqpu.com

[J06] 计算两时间之差
来源：http://yap.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://enk.yuxming.cn

PHP:  $end->diff($start)->days;
来源：http://lya.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vmq.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pdz.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://xul.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://jwr.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://wud.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://qlx.guowangkeji.top

[J07] 比较两个日期
来源：http://gcb.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://dya.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dxr.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://wes.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://kqo.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://edz.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zzq.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://ykc.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://afs.nanxinkj.top

[J08] 提取年月日与星期
来源：http://wlb.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ovt.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qko.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hpe.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ddj.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gpg.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ayn.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zzx.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cfs.nanxuanxn.top

[J09] 时区处理
来源：http://cvo.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mfv.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vkt.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://viq.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://odk.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ttk.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wyg.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vzt.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ofa.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://ppn.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://dwt.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mjn.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bed.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zqz.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ppl.bjfxy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lub.dashuyun.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rxe.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zcb.xuanzx.com

================================================================================
来源：http://cdv.cucudq.cn

K. JSON 与序列化
来源：http://kxt.xingfuxueyuan.xyz

================================================================================
来源：http://ecz.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://xgd.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tle.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jla.kuanghao11.cn

JS:   JSON.stringify(obj)
来源：http://fme.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://azp.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vtm.wangdashe.top

Go:   json.Marshal(obj)
来源：http://yjd.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://utv.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xvb.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://xpc.gzhubu.top

Py:   json.loads(s)
来源：http://pwl.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wbb.gotoacloud.top

JS:   JSON.parse(s)
来源：http://lho.guowangkeji.top

TS:   JSON.parse(s)
来源：http://wts.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yxw.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://szr.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://otc.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xqz.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://tcq.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oyc.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://otd.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://umk.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nqc.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://drl.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://snj.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://aec.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cjw.pycfn.com

[K04] 读取 JSON 文件
来源：http://gph.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vls.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lzn.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sfa.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gwm.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zfm.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vqq.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gnl.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cdk.ppjwa.cn

[K05] 深拷贝对象
来源：http://bor.zhengqikj.top

Py:   copy.deepcopy(obj)
来源：http://iwb.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://gmv.tanke756.top

JS:   structuredClone(obj)
来源：http://prl.zycfv.cn

TS:   structuredClone(obj)
来源：http://owl.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xsw.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://voy.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hek.yj20258888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ytj.yj20258.top

[K06] 解析 URL 查询串
来源：http://jpu.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tcu.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zdc.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mgy.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ple.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://caq.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ebu.zhoulong.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kyd.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gpt.shanyushiyangkeji.top

[K07] 进制转换
来源：http://dbh.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hxu.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dai.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://agx.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://abz.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iav.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://skv.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yfx.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://umc.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://bex.jinyuanbaomall.cn

Py:   pickle.dumps(obj)
来源：http://zfq.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://brq.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://pht.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://fwo.zhoulong.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ofg.svipenyu.cn

Go:   encoding/gob
来源：http://jay.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://njx.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ock.wangdashe.top

================================================================================
来源：http://tbm.hnxiangtu.top

L. 网络请求
来源：http://skp.jlsjyb.cn

================================================================================
来源：http://bzj.jianghu66.top

[L01] 发送 GET 请求
来源：http://qzy.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nuv.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nay.guowangkeji.top

JS:   await fetch(url)
来源：http://ymq.xziqi.cn

TS:   await fetch(url)
来源：http://odg.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mxa.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://iul.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hsu.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tvp.xziqi.cn

[L02] 发送 POST JSON
来源：http://lwv.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://lzy.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fwo.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cwr.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vhy.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vga.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vml.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kfe.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hzm.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://nox.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pxt.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://alg.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fhp.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nbe.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://phg.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ifk.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sxp.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sae.haohaochexian.top

[L04] 设置超时
来源：http://ity.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://kbs.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dzw.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tjf.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fgi.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sfr.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xhc.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://thl.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mhc.xuanzx.com

[L05] 上传文件（multipart）
来源：http://zyv.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uyz.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://phz.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://klb.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://men.ehwqpu.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ngi.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zpd.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://naa.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zjf.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://mzv.ywan-chungtsiang.top

Py:   resp.json()
来源：http://fes.wangdashe.top

PHP:  json_decode($body, true);
来源：http://tgn.redwolf501.top

JS:   await resp.json()
来源：http://tvx.zhengqikj.top

TS:   await resp.json()
来源：http://yef.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bjr.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ifa.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://qdn.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mrw.zhengqikj.top


<!-- 参考信息 -->