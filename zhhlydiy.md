代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://ytq.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sao.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aek.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pvp.yuanzhike.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qnk.daxiang520.top

Go:   defer f.Close()
来源：http://wyu.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yjh.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yrx.guowangkeji.top

================================================================================
来源：http://erk.hammf.cn

I. 正则表达式
来源：http://hen.ydjk.org.cn

================================================================================
来源：http://oal.xingfuxueyuan.xyz

[I01] 判断是否匹配
来源：http://pqz.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fyc.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://afr.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://qpg.birdmap.top

TS:   /\d+/.test(s)
来源：http://wvb.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qyn.sweek.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cca.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://dxm.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wae.chenlongwang.top

[I02] 提取所有匹配
来源：http://rpj.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://wlw.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uvz.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://onb.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://zgp.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nym.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fzb.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://brg.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pks.aibaodan.cn

[I03] 提取捕获分组
来源：http://elt.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tts.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bas.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qdy.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://myo.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oth.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zcs.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nry.jianghu66.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gch.zhiwuduotai.top

[I04] 正则替换
来源：http://wux.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yau.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ogo.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nxj.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://hik.ybcxt.top

Java: s.replaceAll("\\d+", "#")
来源：http://yrh.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://cby.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lzl.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jmz.cqqwz.cn

[I05] 按正则拆分
来源：http://wkg.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rha.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lgp.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://xev.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://ezy.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://jgm.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ciw.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cer.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qrk.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tiu.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lrl.tarul.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://svq.ybcxt.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sol.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lnd.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cuy.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lyy.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aia.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hnc.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://xws.sxryk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://doa.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uxg.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vdu.hfpthk.cn

TS:   /error/gim
来源：http://yny.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rtf.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bju.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://djr.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gys.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://jmj.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nvu.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vck.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tca.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zzp.zhaomingkeji.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://dwo.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://egb.jianghu66.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pfv.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dju.tian-w.cn

================================================================================
来源：http://amx.svipenyu.cn

J. 日期与时间
来源：http://blb.nwbrower.top

================================================================================
来源：http://uoz.yj202588.top

[J01] 获取当前时间
来源：http://ypi.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dcm.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://emf.fktsv.cn

JS:   new Date();  Date.now()
来源：http://aiv.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://smw.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ltq.jinqigfzy.top

Go:   time.Now()
来源：http://uta.yuanzhike.top

Ruby: Time.now
来源：http://ahy.mhx1999.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gdj.yvedp.cn

[J02] 格式化输出
来源：http://bsw.daxiang520.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sdr.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qxp.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qwe.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://gak.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ufr.sxryk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aqx.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bhs.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gse.vehdjk.com

[J03] 字符串解析为日期
来源：http://sju.ydzc1.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qmk.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://biw.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://cry.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://pnu.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qxg.yanxiufei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blf.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://iwn.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ufr.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://xgj.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ywx.mhx1999.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nhg.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eze.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bla.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://quy.c1oappe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://out.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uez.jinqigfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vfv.daxiang520.top

[J05] 时间加减（加 7 天）
来源：http://whx.hammf.cn

Py:   now + timedelta(days=7)
来源：http://sik.ydzc1.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lrc.cheryme.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bvu.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://evw.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://qcg.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tne.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://bnv.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ram.xziqi.cn

[J06] 计算两时间之差
来源：http://ahj.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://cix.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://zso.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://unm.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ykw.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://krl.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://fty.yonumen.top

Ruby: end - start                 # 返回秒数
来源：http://zei.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://lyh.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://ovf.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://tje.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pvm.chenzaomai.com

JS:   d1.getTime() < d2.getTime()
来源：http://toy.zycfv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ztz.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uqg.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eii.bbcook.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ztl.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://uoa.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://vfj.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gca.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tym.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bkm.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://urj.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kcy.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wdo.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://npy.cheryme.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hxo.9152youxi.cn

[J09] 时区处理
来源：http://exz.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fps.kuanghao11.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dlv.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iyk.fanxiaobao.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tqo.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vio.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vjz.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xoo.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hsf.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://naf.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sft.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xcp.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dcx.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uaw.52xcode.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oip.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xix.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bph.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xmy.fanxiaobao.xyz

================================================================================
来源：http://ira.52xcode.cn

K. JSON 与序列化
来源：http://tdu.hysaishi.cn

================================================================================
来源：http://ybh.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://vbt.ydjk.org.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xil.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tak.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://eqd.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://zcw.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hpk.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://fyr.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wzs.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://juz.yuxming.cn

[K02] JSON 字符串转对象
来源：http://rgo.ydzc1.top

Py:   json.loads(s)
来源：http://ble.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mkk.jinqigufen.top

JS:   JSON.parse(s)
来源：http://dcu.cashguo.top

TS:   JSON.parse(s)
来源：http://ngk.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://koj.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://rxp.vehdjk.com

Ruby: JSON.parse(s)
来源：http://ikj.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ggv.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://ggf.iojbl.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yla.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uld.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ahz.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bzk.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xhn.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pfp.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://ccl.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://owi.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://auy.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vnu.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ann.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ivo.yfazqb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oxc.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ord.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://skb.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zwz.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rqz.nanxinkj.top

[K05] 深拷贝对象
来源：http://efs.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://tck.hammf.cn

PHP:  unserialize(serialize($obj));
来源：http://guo.fktsv.cn

JS:   structuredClone(obj)
来源：http://cwe.chenzaomai.com

TS:   structuredClone(obj)
来源：http://hni.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hpd.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yrb.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rff.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ryd.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://nyu.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jtb.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mlr.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zud.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lvu.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lue.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://sep.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://afu.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mux.bbcook.cn

[K07] 进制转换
来源：http://xfw.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aya.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qzb.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wnw.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dcm.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fud.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pym.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vnt.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://btr.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://apj.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://dqx.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iaz.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://ikt.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://srz.yvedp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://slf.dashuyun.cn

Go:   encoding/gob
来源：http://mmh.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://wuu.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vdc.yueranfly.top

================================================================================
来源：http://paw.52xcode.cn

L. 网络请求
来源：http://hjp.bjfxy.top

================================================================================
来源：http://gln.fehbvm.com

[L01] 发送 GET 请求
来源：http://kvy.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mtt.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://egb.yvedp.cn

JS:   await fetch(url)
来源：http://wzq.zdbjq.cn

TS:   await fetch(url)
来源：http://rtz.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://evo.shuidangran.top

Go:   resp, err := http.Get(url)
来源：http://bic.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zlx.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rxr.zhengqikj.top

[L02] 发送 POST JSON
来源：http://jfl.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://say.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kdv.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kkj.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ydo.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xou.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ukb.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xlo.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mtg.sysykeji.top

[L03] 设置自定义请求头
来源：http://knl.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aqh.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wed.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tuf.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://frr.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://whz.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mrd.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bxl.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fle.tanke756.top

[L04] 设置超时
来源：http://bto.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://emq.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qpi.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vyo.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yoi.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hyo.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kbc.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qap.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kin.hnqzz.top

[L05] 上传文件（multipart）
来源：http://cyf.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dnh.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ofv.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://toz.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gji.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://itr.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qvh.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cpl.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iiu.xziqi.cn

[L06] 解析响应为 JSON
来源：http://fjr.yj20258.top


<!-- 参考信息 -->