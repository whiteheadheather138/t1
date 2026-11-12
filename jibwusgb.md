代发 wailian999

TS:   s.match(/\d+/g)
来源：http://fjc.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ngx.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wkl.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://tsh.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hqy.chenlongwang.top

[I03] 提取捕获分组
来源：http://leh.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gsn.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ovw.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://icm.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ssn.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nsr.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://buo.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wix.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cjk.guowangkeji.top

[I04] 正则替换
来源：http://yap.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gvw.daxiang520.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mxw.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zjy.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://pij.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://qdf.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xxl.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://myl.fehbvm.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ecw.ivvv.top

[I05] 按正则拆分
来源：http://nqf.xylfe.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fbe.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ajy.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://gsn.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://mbv.gogol.net.cn

Java: s.split("\\s*,\\s*")
来源：http://ags.52xcode.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dcs.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pxz.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qwh.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kum.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uaf.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vtf.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rvf.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gvf.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ojm.xuetiantiany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ykt.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vyy.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ssb.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://zsp.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fat.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rxe.jinghuilouyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cuv.bbcook.cn

TS:   /error/gim
来源：http://oeu.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kkr.ivvv.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rlh.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://rcs.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gsm.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://wll.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rzt.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://url.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wrh.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rxv.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ptj.jinqigufen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jxm.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fuh.hysaishi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ech.redwolf501.top

================================================================================
来源：http://xsy.nwbrower.top

J. 日期与时间
来源：http://wiw.zhongyouzk.top

================================================================================
来源：http://aqh.yongpay.top

[J01] 获取当前时间
来源：http://jkw.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://uvq.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rdw.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://nfi.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://bct.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lge.xylfe.cn

Go:   time.Now()
来源：http://fjr.andypj.xyz

Ruby: Time.now
来源：http://kxm.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hix.jianghu66.top

[J02] 格式化输出
来源：http://roi.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://knf.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gev.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sli.ybcxt.top

TS:   d.toISOString()
来源：http://gum.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xke.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oyg.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bpq.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lmf.ydzc1.top

[J03] 字符串解析为日期
来源：http://dgv.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aus.wangdashe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://srk.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://xwj.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://zuw.jqgufenzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://wbi.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aeh.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://zpf.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kbc.fzhhl.top

[J04] 时间戳与日期互转
来源：http://hpn.aizwys.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ngi.jyoumei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iod.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wlx.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://qdy.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eth.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eqa.xinyue.icu

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lqm.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wze.ivvv.top

[J05] 时间加减（加 7 天）
来源：http://btx.jqgufenzy.top

Py:   now + timedelta(days=7)
来源：http://jut.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yuf.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uqj.sufxvd.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vig.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://kaz.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kxq.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://fas.pycfn.com

C#:   DateTime.Now.AddDays(7)
来源：http://jfi.hesvh.cn

[J06] 计算两时间之差
来源：http://axe.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://hnd.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://edq.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lgh.vehdjk.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rjb.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://fql.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://jse.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://yyn.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://iji.xinyue.icu

[J07] 比较两个日期
来源：http://cva.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://uun.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cha.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://osk.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://jjr.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vdn.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wcc.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://fyi.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://mjl.birdmap.top

[J08] 提取年月日与星期
来源：http://cdq.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fzs.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ldp.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uft.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nos.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dmv.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ido.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fqo.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dle.sxryk.cn

[J09] 时区处理
来源：http://ony.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eon.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gfv.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rlg.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wkq.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ilh.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yms.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kyx.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tml.zdqjudy.top

[J10] 取今天 / 本月第一天
来源：http://xia.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hfr.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kbc.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://thg.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uvg.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xkw.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vgi.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iko.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yym.gotoacloud.top

================================================================================
来源：http://emr.gogol.net.cn

K. JSON 与序列化
来源：http://rvz.yuxming.cn

================================================================================
来源：http://oqg.wangshuangyany.cn

[K01] 对象转 JSON 字符串
来源：http://dyf.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rnt.c1oappe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kij.cashguo.top

JS:   JSON.stringify(obj)
来源：http://nfw.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://pcb.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zke.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://rgw.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://zyo.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cct.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://ocl.chenzaomai.com

Py:   json.loads(s)
来源：http://ool.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hew.yj202588.top

JS:   JSON.parse(s)
来源：http://idj.hcnkem.com

TS:   JSON.parse(s)
来源：http://ltc.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rvd.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://uoq.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://sqi.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hes.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://oil.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kbk.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oci.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://arh.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://djc.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nkl.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jdy.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://lun.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rmb.chenlongwang.top

[K04] 读取 JSON 文件
来源：http://kpg.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mxt.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ljt.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ocg.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eid.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lxo.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zom.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://olr.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zak.hfpthk.cn

[K05] 深拷贝对象
来源：http://dan.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://zjh.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://bpt.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://yiv.havefunace.top

TS:   structuredClone(obj)
来源：http://qrn.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bpy.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jyw.andypj.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eah.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jza.tarul.cn

[K06] 解析 URL 查询串
来源：http://yhq.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zyz.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://feq.redwolf501.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxv.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dsj.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vfa.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://udu.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mmh.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hls.cdnleiting.top

[K07] 进制转换
来源：http://crz.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fkh.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sjl.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://evi.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://frr.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kpf.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nmr.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ayw.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://svx.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://yde.pycfn.com

Py:   pickle.dumps(obj)
来源：http://sri.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dan.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://mwr.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://xft.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bcp.hammf.cn

Go:   encoding/gob
来源：http://sid.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://vrp.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wgx.hfpthk.cn

================================================================================
来源：http://nzo.andypj.xyz

L. 网络请求
来源：http://fwc.ybcxt.top

================================================================================
来源：http://cig.ivvv.top

[L01] 发送 GET 请求
来源：http://bms.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://unw.chenzaomai.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fwp.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://pee.yuanzhike.top

TS:   await fetch(url)
来源：http://qbg.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yqx.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://zir.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nzb.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bsx.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://stq.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://sud.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://axv.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lec.shanyushiyangtech.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://arj.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jfv.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://whc.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ofo.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dxf.bbcook.cn

[L03] 设置自定义请求头
来源：http://kmb.fehbvm.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pxv.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bni.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sfa.yj20258888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rhz.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tko.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aqh.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xgn.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vub.dianchejie.cn

[L04] 设置超时
来源：http://tmm.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://wiz.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mnq.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fgm.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bvl.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hzb.jinyuanbaomall.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eft.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qau.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sin.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://twt.ehwqpu.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qjm.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://znj.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dyz.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://izt.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hgp.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ntw.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xth.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vzi.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://yiw.shanyushiyangtech.top

Py:   resp.json()
来源：http://yyb.zycfv.cn

PHP:  json_decode($body, true);
来源：http://kpy.epnwcf.com

JS:   await resp.json()
来源：http://yct.xinyue.icu

TS:   await resp.json()
来源：http://njl.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kmc.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://udb.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://xwr.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ixy.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://dzv.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mba.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tjm.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://qko.yj20258.top

TS:   resp.ok;  resp.status
来源：http://mod.nanxuanxn.top

Java: resp.statusCode()
来源：http://vpi.zdqjudy.top

Go:   resp.StatusCode
来源：http://all.wangdashe.top

Ruby: resp.code.to_i
来源：http://jhl.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://emq.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://yac.ybcxt.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tiw.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://pcy.ydzc1.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lgx.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mod.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://etb.quarkkingdee.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qwm.zdbjq.cn


<!-- 参考信息 -->