代发 wailian999

TS:   s.match(/\d+/g)
来源：http://ate.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gqw.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bzk.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://ezo.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ddd.hfpthk.cn

[I03] 提取捕获分组
来源：http://npp.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xhq.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dpl.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://epx.zhoulong.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iex.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jvp.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lfr.hesvh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://egk.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wte.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://cut.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dnf.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://irg.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://aal.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://yxu.zhongyouzk.top

Java: s.replaceAll("\\d+", "#")
来源：http://pju.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://vdz.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://spv.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ear.jinghuilouyu.cn

[I05] 按正则拆分
来源：http://wub.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lwl.bjfxy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ffl.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://zdc.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://lul.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://imn.hesvh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sxt.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sou.jlsjyb.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://apt.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zpc.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dlx.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nxb.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yue.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uzc.pengpengdd.cyou

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cwn.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eps.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://csf.sysykeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dah.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://lxp.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rex.c1oappe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blw.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tmb.nanxuanxn.top

TS:   /error/gim
来源：http://enh.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wnd.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zrv.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://pcl.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cax.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://grl.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bgy.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cxg.tarul.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uer.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lrr.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wuc.hywenlv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rgm.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qnt.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lfp.aibaodan.cn

================================================================================
来源：http://oia.andypj.xyz

J. 日期与时间
来源：http://vsz.shanyushiyangkeji.top

================================================================================
来源：http://lnp.yvedp.cn

[J01] 获取当前时间
来源：http://frn.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qrp.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kha.xinyue.icu

JS:   new Date();  Date.now()
来源：http://zbv.yj202588.top

TS:   new Date();  Date.now()
来源：http://jzy.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xlb.yuxming.cn

Go:   time.Now()
来源：http://pgx.guowangkeji.top

Ruby: Time.now
来源：http://hwk.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://itx.shuidangran.top

[J02] 格式化输出
来源：http://kvn.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vcw.wangdashe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rih.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cju.guowangkeji.top

TS:   d.toISOString()
来源：http://pjn.bjfxy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://err.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://anm.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wua.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wje.ydzc1.top

[J03] 字符串解析为日期
来源：http://lry.yj20258888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://swy.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vym.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://blx.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://way.cdnleiting.top

Java: LocalDate.parse("2024-01-02")
来源：http://dsz.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fwc.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://pwj.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://idf.meibo888.top

[J04] 时间戳与日期互转
来源：http://vdr.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jyr.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dqw.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sed.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://diu.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sep.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xqo.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://grf.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dgx.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://bie.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://ibd.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rwn.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://igm.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vdb.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://qyl.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xxu.yonumen.top

Ruby: Time.now + 7 * 86400
来源：http://qmd.sjlbkw.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qwn.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://kwb.cheryme.top

Py:   (end - start).total_seconds()
来源：http://jbn.jinqigufen.top

PHP:  $end->diff($start)->days;
来源：http://zry.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dtj.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rwx.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://lue.tianlin.xyz

Go:   end.Sub(start).Hours()
来源：http://ett.xinyue.icu

Ruby: end - start                 # 返回秒数
来源：http://xbg.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://vxq.bbcook.cn

[J07] 比较两个日期
来源：http://imx.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://uhj.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qcn.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mow.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://yad.redwolf501.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xzy.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ana.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nhn.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://ubx.zhengqikj.top

[J08] 提取年月日与星期
来源：http://zry.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nnk.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rdw.jqgufenzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sxg.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://spg.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jql.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gmy.yuanzhike.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jmh.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://atr.9152youxi.cn

[J09] 时区处理
来源：http://hrp.pengpengdd.cyou

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dnx.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vcd.jqgfzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emh.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jmb.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://chf.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://txs.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qtb.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tmg.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://jlo.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nvc.sysykeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dlp.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://txl.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://plb.jqgfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rau.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hsq.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mmr.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aqh.ydjk.org.cn

================================================================================
来源：http://hcg.yanxiufei.cn

K. JSON 与序列化
来源：http://zox.shangyingyoupin.top

================================================================================
来源：http://dmz.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://kcl.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ujg.shzxlz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://swl.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://whk.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://pyt.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hqw.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://bkk.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://jue.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://pch.hesvh.cn

[K02] JSON 字符串转对象
来源：http://mld.jlsjyb.cn

Py:   json.loads(s)
来源：http://phj.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gmo.jiagoushi.top

JS:   JSON.parse(s)
来源：http://cpm.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://bji.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qyq.hammf.cn

Go:   json.Unmarshal(data, &v)
来源：http://nww.sysykeji.top

Ruby: JSON.parse(s)
来源：http://rnr.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wda.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://vky.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kdh.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://itm.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kjx.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lkb.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qij.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kio.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uio.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lqu.aizwys.cn

[K04] 读取 JSON 文件
来源：http://qkx.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dyu.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jdw.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qzs.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jjy.gotoacloud.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dii.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aks.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://see.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lab.sxryk.cn

[K05] 深拷贝对象
来源：http://pkn.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://fuc.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://jvq.zdbjq.cn

JS:   structuredClone(obj)
来源：http://wkw.daxiang520.top

TS:   structuredClone(obj)
来源：http://sgt.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://iqy.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mzx.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zsf.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://dsx.fktsv.cn

[K06] 解析 URL 查询串
来源：http://wcz.hnxiangtu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pjj.smart0.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qai.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ulr.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ert.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mtt.fzhhl.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jrd.guannengcc.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wyj.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rnd.dianchejie.cn

[K07] 进制转换
来源：http://vzu.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://epo.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://icy.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xfx.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nit.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nxa.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ubw.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://anb.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ofk.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://yaw.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://uep.shzxlz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lfl.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://wmj.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://jlr.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://igh.hesvh.cn

Go:   encoding/gob
来源：http://ygk.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://evf.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://stn.andypj.xyz

================================================================================
来源：http://ods.andypj.xyz

L. 网络请求
来源：http://evk.nwbrower.top

================================================================================
来源：http://spr.ctjpmb.com

[L01] 发送 GET 请求
来源：http://ies.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://las.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zra.bjfxy.top

JS:   await fetch(url)
来源：http://evd.epnwcf.com

TS:   await fetch(url)
来源：http://cge.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ybk.jyoumei.cn

Go:   resp, err := http.Get(url)
来源：http://hwd.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://src.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jgi.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://mui.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://zcb.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://siv.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://axo.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kis.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jhu.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zjt.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zad.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ygs.ydzc1.top

[L03] 设置自定义请求头
来源：http://jma.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mts.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yto.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cmn.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tfn.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kam.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://diz.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ffa.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jib.jinghuilouyu.cn

[L04] 设置超时
来源：http://vzi.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://axv.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zze.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://trs.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iue.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rlm.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mco.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lom.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rzf.ivvv.top

[L05] 上传文件（multipart）
来源：http://tsu.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bku.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uqr.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dhp.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yqu.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dxo.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://igm.yj202588.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ffz.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lwp.yfazqb.com

[L06] 解析响应为 JSON
来源：http://kgn.hammf.cn

Py:   resp.json()
来源：http://qlg.fzhhl.top

PHP:  json_decode($body, true);
来源：http://fwg.zdbjq.cn

JS:   await resp.json()
来源：http://sas.zdqjudy.top

TS:   await resp.json()
来源：http://yvj.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eyr.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hsu.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://ctv.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://flu.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://vnh.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vov.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gkf.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://gnw.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://eia.zhijiandao.cn

Java: resp.statusCode()
来源：http://dcp.hywenlv.cn

Go:   resp.StatusCode
来源：http://isj.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://ema.yongpay.top

C#:   (int)resp.StatusCode
来源：http://vhn.tanke756.top

[L08] 并发请求多个地址
来源：http://krc.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://swe.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://pgq.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oes.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xjl.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lan.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fkc.chenlongwang.top


<!-- 参考信息 -->