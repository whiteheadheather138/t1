代发 wailian999

TS:   s.match(/\d+/g)
来源：http://ced.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bld.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://peb.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://tat.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gby.epnwcf.com

[I03] 提取捕获分组
来源：http://iqu.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qkz.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bvq.sxryk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://akf.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://the.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://abs.0kj1m.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qiq.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lzh.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xmp.xziqi.cn

[I04] 正则替换
来源：http://tgp.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vuq.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aly.sweek.top

JS:   s.replace(/\d+/g, "#")
来源：http://dkf.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hbj.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://hia.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://urt.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jqm.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ckf.bjfxy.top

[I05] 按正则拆分
来源：http://vqo.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kux.redwolf501.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://odq.yj202588.top

JS:   s.split(/\s*,\s*/)
来源：http://wci.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://tzx.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://iak.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lbx.redwolf501.top

Ruby: s.split(/\s*,\s*/)
来源：http://pod.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://enh.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wsg.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jhh.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ydn.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qfq.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nks.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wez.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pbi.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ebc.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fry.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://ndw.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rhj.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vqu.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bsx.tian-w.cn

TS:   /error/gim
来源：http://xtn.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nix.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://utj.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://tyf.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eoz.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://nzt.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tng.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cpl.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lja.fzhhl.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wrz.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ptc.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nfy.jianghu66.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://clp.tianlin.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://knr.52xcode.cn

================================================================================
来源：http://qcp.xylfe.cn

J. 日期与时间
来源：http://yvo.daria6918.cn

================================================================================
来源：http://brk.0kj1m.cn

[J01] 获取当前时间
来源：http://mgd.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://rmh.vqdsnc.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ozp.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://wcu.gogol.net.cn

TS:   new Date();  Date.now()
来源：http://qha.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ilf.yfazqb.com

Go:   time.Now()
来源：http://qdt.snrcjt.cn

Ruby: Time.now
来源：http://twd.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mdd.zhiwuduotai.top

[J02] 格式化输出
来源：http://jgg.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ozb.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lnp.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yim.fktsv.cn

TS:   d.toISOString()
来源：http://rrs.dashuyun.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qae.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rid.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gsb.meibo888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://emw.yvedp.cn

[J03] 字符串解析为日期
来源：http://yhb.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bvq.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xbl.zhixingplan.top

JS:   new Date("2024-01-02")
来源：http://jkd.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://bjk.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uxe.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yqv.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ajd.uphjek.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ppm.yfazqb.com

[J04] 时间戳与日期互转
来源：http://mex.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vov.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xsx.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ttp.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://tly.svipenyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cot.iojbl.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eie.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://inb.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://guj.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://yba.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://nbp.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://otb.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://emx.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://elu.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://cah.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hop.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://hxv.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://vid.yuxming.cn

[J06] 计算两时间之差
来源：http://ddn.xuanzx.com

Py:   (end - start).total_seconds()
来源：http://olg.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://opm.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://whx.yvedp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yfx.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pza.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://bbq.jianghu66.top

Ruby: end - start                 # 返回秒数
来源：http://wwa.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://mrf.svipenyu.cn

[J07] 比较两个日期
来源：http://pvq.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://xek.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xxs.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://akx.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://hbi.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iho.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tbs.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://dhg.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://krs.meibo888.top

[J08] 提取年月日与星期
来源：http://vbi.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fjr.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gnu.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ppo.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bzy.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eif.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://our.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vim.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://iul.zhongyouzk.top

[J09] 时区处理
来源：http://cow.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dxa.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://doa.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nvi.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dyo.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bqs.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zjf.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://scr.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hds.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://wkn.aibaodan.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://duq.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kvk.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cqi.xingfuxueyuan.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mtb.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qlf.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vkm.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kro.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hal.fehbvm.com

================================================================================
来源：http://twy.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://kvy.52xcode.cn

================================================================================
来源：http://whf.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://tse.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fkl.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ipr.jqgfzy.top

JS:   JSON.stringify(obj)
来源：http://vlm.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://lbm.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ldb.havefunace.top

Go:   json.Marshal(obj)
来源：http://fcd.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://pua.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ufa.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://sfl.aibaodan.cn

Py:   json.loads(s)
来源：http://kye.nwbrower.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mrc.0kj1m.cn

JS:   JSON.parse(s)
来源：http://qxg.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://suw.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://djh.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://pfa.havefunace.top

Ruby: JSON.parse(s)
来源：http://hji.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xok.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://iqo.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bmn.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://swh.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fsh.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mmj.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ggm.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://msz.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://nyq.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kdn.yfazqb.com

[K04] 读取 JSON 文件
来源：http://eea.hywenlv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ctl.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nav.jianghu66.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://egx.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hek.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://niv.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qns.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zbn.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ojb.jiagoushi.top

[K05] 深拷贝对象
来源：http://wrn.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://nzn.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://jvv.gzhubu.top

JS:   structuredClone(obj)
来源：http://qam.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://you.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yvm.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sxc.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://exs.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://vaf.yueranfly.top

[K06] 解析 URL 查询串
来源：http://rwo.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jvr.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://efy.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pha.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eed.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jtp.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://enw.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cjv.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://urx.ctjpmb.com

[K07] 进制转换
来源：http://coe.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ktb.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rrd.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rit.wangshuangyany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ucg.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fjr.hcnkem.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gnh.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eqq.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kdz.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://tco.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://svq.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pgh.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://its.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://jde.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vcs.hfpthk.cn

Go:   encoding/gob
来源：http://rsj.hywenlv.cn

Ruby: Marshal.dump(obj)
来源：http://lzl.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yav.pycfn.com

================================================================================
来源：http://rsj.tarul.cn

L. 网络请求
来源：http://amq.yj202588.top

================================================================================
来源：http://nvu.vehdjk.com

[L01] 发送 GET 请求
来源：http://ioi.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jqt.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ijp.meibo888.top

JS:   await fetch(url)
来源：http://rvf.feifeiyinyue.top

TS:   await fetch(url)
来源：http://wvr.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ank.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://det.vqdsnc.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://erp.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ige.cucudq.cn

[L02] 发送 POST JSON
来源：http://ckj.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://doj.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jqa.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pxl.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ien.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sno.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mgi.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aaz.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hcn.tanke756.top

[L03] 设置自定义请求头
来源：http://lwz.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://koc.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yxm.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aow.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://isy.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mqm.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mng.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fvx.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xmw.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://slo.smart0.xyz

Py:   requests.get(url, timeout=5)
来源：http://ijf.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fbv.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rti.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fjr.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lmz.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://llh.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aar.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kgj.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://dmy.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dqt.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oml.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jmu.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vfq.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jma.tarul.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ufq.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://etx.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vvo.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://dvi.sysykeji.top

Py:   resp.json()
来源：http://ike.cucudq.cn

PHP:  json_decode($body, true);
来源：http://tmr.guowangkeji.top

JS:   await resp.json()
来源：http://klx.fengsongda.top

TS:   await resp.json()
来源：http://obk.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qym.zhengqikj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cbv.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://nda.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wsx.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://ofd.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tbn.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://azn.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://mwm.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://kqt.tarul.cn

Java: resp.statusCode()
来源：http://qdh.redwolf501.top

Go:   resp.StatusCode
来源：http://pbr.tarul.cn

Ruby: resp.code.to_i
来源：http://vch.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://crh.tian-w.cn

[L08] 并发请求多个地址
来源：http://iyh.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ruf.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://gwm.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://asd.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hxf.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tlv.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pln.yanxiufei.cn


<!-- 参考信息 -->