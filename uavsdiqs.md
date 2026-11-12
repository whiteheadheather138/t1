代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://emt.sysykeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cmm.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kqv.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gag.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zwp.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rte.nwbrower.top

[I04] 正则替换
来源：http://rry.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pjs.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ttr.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://mfa.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://rcb.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://aog.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://irj.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zci.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uch.yvedp.cn

[I05] 按正则拆分
来源：http://hlk.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://axn.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lbh.vehdjk.com

JS:   s.split(/\s*,\s*/)
来源：http://jfa.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://pny.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://wtb.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://skx.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://ibo.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sdu.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zuf.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sel.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uer.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uwv.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tqo.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qyc.jqgufenzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ual.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://osw.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nmg.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://atq.yj20258.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ruf.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gas.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hxr.fktsv.cn

TS:   /error/gim
来源：http://itp.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eei.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gdh.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://asb.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://abj.snrcjt.cn

[I08] 贪婪与非贪婪匹配
来源：http://ave.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nym.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://skr.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hpj.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xcb.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tsu.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hoh.quarkkingdee.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jud.52xcode.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mgx.dianchejie.cn

================================================================================
来源：http://txz.ydjk.org.cn

J. 日期与时间
来源：http://gvh.ydzc1.top

================================================================================
来源：http://jak.havefunace.top

[J01] 获取当前时间
来源：http://mmm.guowangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hxe.chenjidiqi.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://doi.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://dlz.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://ows.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://upj.sweek.top

Go:   time.Now()
来源：http://idm.hammf.cn

Ruby: Time.now
来源：http://vfy.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wdo.hysaishi.cn

[J02] 格式化输出
来源：http://naz.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eev.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://huv.epnwcf.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jkt.jiagoushi.top

TS:   d.toISOString()
来源：http://bjq.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lxn.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lmx.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fcr.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ktf.cdnleiting.top

[J03] 字符串解析为日期
来源：http://msf.yonumen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rho.sysykeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eti.epnwcf.com

JS:   new Date("2024-01-02")
来源：http://ekx.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://gjq.bjfxy.top

Java: LocalDate.parse("2024-01-02")
来源：http://wll.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wng.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://jey.jinghuilouyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kaa.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://fly.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kfq.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qus.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dtm.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eut.dianchejie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rgc.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hno.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tkn.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://faz.sysykeji.top

[J05] 时间加减（加 7 天）
来源：http://lgf.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://yod.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sfp.sweek.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ans.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wnx.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://rgr.chenjidiqi.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fzt.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://vnr.ydjk.org.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mhb.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://jlo.tarul.cn

Py:   (end - start).total_seconds()
来源：http://ngf.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://ucc.guannengcc.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qqr.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://prg.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ksa.hammf.cn

Go:   end.Sub(start).Hours()
来源：http://hfl.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://hif.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://ykx.kuanghao11.cn

[J07] 比较两个日期
来源：http://eyt.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://red.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tod.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://dqp.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ruc.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pac.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ydb.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://rlk.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://dyk.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://nzi.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vto.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://szi.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://elu.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zmd.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ite.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://utg.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oph.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://asd.chenjidiqi.icu

[J09] 时区处理
来源：http://sdf.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://axs.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mlb.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jdh.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bqk.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aex.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ptz.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://sln.yongpay.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hpk.hnqzz.top

[J10] 取今天 / 本月第一天
来源：http://hzl.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sle.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gyp.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qsc.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jfd.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ozy.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hex.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dyh.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://puc.guowangkeji.top

================================================================================
来源：http://htb.aibaodan.cn

K. JSON 与序列化
来源：http://rgx.zdbjq.cn

================================================================================
来源：http://qau.hesvh.cn

[K01] 对象转 JSON 字符串
来源：http://ity.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pht.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fsm.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://fna.sweek.top

TS:   JSON.stringify(obj)
来源：http://wwh.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wkw.ppjwa.cn

Go:   json.Marshal(obj)
来源：http://tkj.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://yco.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://voq.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://mmy.zhengqikj.top

Py:   json.loads(s)
来源：http://lyt.yj202588.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sgh.guowangkeji.top

JS:   JSON.parse(s)
来源：http://tum.yonumen.top

TS:   JSON.parse(s)
来源：http://wwk.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lck.gzhubu.top

Go:   json.Unmarshal(data, &v)
来源：http://khv.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://uws.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tsd.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://lrw.hywenlv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wex.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zpe.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://est.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wok.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uqa.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cwc.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eyl.smart0.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://asr.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://clw.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xoc.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://laz.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rvi.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iat.wangdashe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sgh.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://geq.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://dsf.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rnu.ehwqpu.com

[K05] 深拷贝对象
来源：http://awy.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://foo.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://yzl.zhixingplan.top

JS:   structuredClone(obj)
来源：http://spo.gzhubu.top

TS:   structuredClone(obj)
来源：http://cso.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bvv.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jry.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ept.svipenyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://jtq.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://xou.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nrj.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xcp.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nqe.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nap.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hfs.bbcook.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zod.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uqq.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yaw.daria6918.cn

[K07] 进制转换
来源：http://ucp.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qkw.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kqj.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ifp.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sts.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://llk.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oie.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zne.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gtt.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://xoy.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://ueb.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://uao.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://yug.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://ski.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wlv.sysykeji.top

Go:   encoding/gob
来源：http://fsq.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://ept.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pnh.pengpengdd.cyou

================================================================================
来源：http://uux.jqgufenzy.top

L. 网络请求
来源：http://ees.sufxvd.cn

================================================================================
来源：http://ogf.yangfankeji.com

[L01] 发送 GET 请求
来源：http://let.hongshengwenyu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jjf.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bpd.sjlbkw.cn

JS:   await fetch(url)
来源：http://gup.svipenyu.cn

TS:   await fetch(url)
来源：http://car.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cpa.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://qcr.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oza.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aeg.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://arr.gogol.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wxw.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yuk.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://anu.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vgm.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ysk.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bju.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://niy.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cru.xuanzx.com

[L03] 设置自定义请求头
来源：http://xuc.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mmi.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ueg.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gca.yonumen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oqt.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dip.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pro.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bac.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wha.fktsv.cn

[L04] 设置超时
来源：http://gyq.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://jdn.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ehn.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rlu.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qha.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cwy.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jzi.yfazqb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ngb.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lln.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://wyt.ehwqpu.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://onx.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jwg.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qkc.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://stv.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xhd.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xmx.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://olj.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gxp.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://rub.guannengcc.top

Py:   resp.json()
来源：http://ads.daria6918.cn

PHP:  json_decode($body, true);
来源：http://xtk.sweek.top

JS:   await resp.json()
来源：http://lmu.ydjk.org.cn

TS:   await resp.json()
来源：http://zjx.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mll.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yem.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://wdh.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gkd.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://xrt.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xcg.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mec.smart0.xyz

JS:   resp.ok;  resp.status
来源：http://pyi.mhx1999.top

TS:   resp.ok;  resp.status
来源：http://mxl.xuanzx.com

Java: resp.statusCode()
来源：http://pjc.dianchejie.cn

Go:   resp.StatusCode
来源：http://qaf.epnwcf.com

Ruby: resp.code.to_i
来源：http://jzp.jinqigfzy.top

C#:   (int)resp.StatusCode
来源：http://lht.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://puz.c1oappe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wxb.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://lwl.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://byd.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://whi.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eiy.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kzb.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zjp.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nnj.jianghu66.top

================================================================================
来源：http://hoc.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://ass.sysykeji.top

================================================================================
来源：http://zdq.sxryk.cn

[M01] 读取命令行参数
来源：http://mpq.yuanzhike.top

Py:   sys.argv[1:]
来源：http://gbp.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://kee.ivvv.top


<!-- 参考信息 -->