代发 wailian999

Py:   isinstance(u, User)
来源：http://iff.aibaodan.cn

PHP:  $u instanceof User
来源：http://gxo.aizwys.cn

JS:   u instanceof User
来源：http://ovb.gogol.net.cn

TS:   u instanceof User
来源：http://ooh.daria6918.cn

Java: u instanceof User
来源：http://gst.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://acx.bjfxy.top

Ruby: u.is_a?(User)
来源：http://via.cdnleiting.top

C#:   u is User
来源：http://dau.fzhhl.top

[G14] 数据类 / record
来源：http://xib.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tyx.shangyingyoupin.top

PHP:  // 用 readonly 属性模拟
来源：http://vpj.fzhhl.top

JS:   // 无内置：普通类或对象字面量
来源：http://llg.svipenyu.cn

TS:   type User = { name: string; age: number };
来源：http://eaq.epnwcf.com

Java: record User(String name, int age) {}
来源：http://hbt.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://zvi.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rof.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://kwo.sufxvd.cn

[G15] 枚举
来源：http://uey.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fjt.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lqs.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bod.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zdm.chenzaomai.com

Java: enum Color { RED, GREEN }
来源：http://avw.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dlu.tianlin.xyz

Ruby: Color = %i[red green].freeze
来源：http://wto.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ijf.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://ywu.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qhs.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://zbf.iojbl.cn

JS:   Object.entries(obj)
来源：http://ufu.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://ijq.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tku.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vsx.zdqjudy.top

Ruby: obj.instance_variables
来源：http://rny.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://mfd.haohaochexian.top

================================================================================
来源：http://wjv.cucudq.cn

H. 异常与错误处理
来源：http://bao.daria6918.cn

================================================================================
来源：http://zhn.zhixingplan.top

[H01] try / catch 基础
来源：http://otw.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lbm.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fbi.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lxx.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dce.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://crb.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kfo.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jto.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vsj.ivvv.top

[H02] finally / ensure 收尾
来源：http://dqs.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wqx.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zfa.sufxvd.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wdt.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yls.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eor.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gir.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://jvh.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iwj.hongshengwenyu.top

[H03] 主动抛出异常
来源：http://fla.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://bju.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zjs.iojbl.cn

JS:   throw new Error("错误信息");
来源：http://oll.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://ipl.316326.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://vlx.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vjb.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vzv.jiagoushi.top

C#:   throw new ArgumentException("错误信息");
来源：http://zkc.zhoulong.xyz

[H04] 自定义异常类型
来源：http://rpy.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://zim.xinyue.icu

PHP:  class MyError extends RuntimeException {}
来源：http://kvk.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://ikd.ydzc1.top

TS:   class MyError extends Error {}
来源：http://vju.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://igb.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ink.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://xwn.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://qgk.yj202588.top

[H05] 捕获特定类型
来源：http://rni.jqgfzy.top

Py:   except ValueError as e:
来源：http://jwd.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qqm.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://lto.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://pwa.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://jmv.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lya.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://ymv.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jfs.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://jvw.jianghu66.top

Py:   value = d.get("k") or default
来源：http://isu.zhiwuduotai.top

PHP:  $v = $d["k"] ?? null;
来源：http://cuy.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://uwf.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://mff.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://alp.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lxg.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://keu.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://vcw.52xcode.cn

[H07] 断言
来源：http://dwl.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://tbf.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://kfa.pycfn.com

JS:   console.assert(x > 0);
来源：http://vcv.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://ffs.gaohongyu789.top

Java: assert x > 0 : "必须为正";
来源：http://bxs.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vhy.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tln.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://fjk.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://yay.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://wlg.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://npg.zdqjudy.top

JS:   e.message;  e.stack
来源：http://lud.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ryd.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gtx.nanxinkj.top

Go:   err.Error()
来源：http://dys.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://cll.pycfn.com

C#:   e.Message;  e.StackTrace
来源：http://kke.tian-w.cn

[H09] 带错误码的异常
来源：http://sob.zhoulong.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dby.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ezl.jinqigfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yik.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kqy.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uub.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lyr.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ams.birdmap.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hrk.jlsjyb.cn

[H10] 资源自动释放
来源：http://jzp.zycfv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qzw.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jsh.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hur.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://irv.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kea.guannengcc.top

Go:   defer f.Close()
来源：http://yod.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ihq.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pea.guannengcc.top

================================================================================
来源：http://sav.zdbjq.cn

I. 正则表达式
来源：http://prs.xylfe.cn

================================================================================
来源：http://kbn.cheryme.top

[I01] 判断是否匹配
来源：http://ric.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gva.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://bnr.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://fzm.fengsongda.top

TS:   /\d+/.test(s)
来源：http://bzp.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cmy.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rcv.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://vsh.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mjv.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://elr.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://fiu.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qmu.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cur.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://giv.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ujk.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pdf.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://rtx.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vhd.xuetiantiany.cn

[I03] 提取捕获分组
来源：http://vym.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://idl.yangfankeji.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kda.zhixingplan.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lhx.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cpe.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://amj.jianghu66.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://atd.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sqy.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wwt.meibo888.top

[I04] 正则替换
来源：http://gdl.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sir.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tte.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://swk.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://btr.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://zhe.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vkc.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cid.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hfb.vqdsnc.cn

[I05] 按正则拆分
来源：http://kxk.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gou.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gym.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://okq.zdqjudy.top

TS:   s.split(/\s*,\s*/)
来源：http://ohj.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://mis.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://weu.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://sba.zhaomingkeji.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zgb.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wwi.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wxv.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gwg.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vur.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nmr.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://agn.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dnv.sweek.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wrx.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rlv.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://ejx.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fcx.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aqj.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jtr.zhongyouzk.top

TS:   /error/gim
来源：http://lge.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ewo.316326.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://amh.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://xzl.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://snf.cqqwz.cn

[I08] 贪婪与非贪婪匹配
来源：http://dlv.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://alj.xziqi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tqr.tian-w.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rkn.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yut.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xfy.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kbs.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rgb.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fhd.shuidangran.top

================================================================================
来源：http://tcr.jinyuanbaomall.cn

J. 日期与时间
来源：http://mlo.sufxvd.cn

================================================================================
来源：http://fug.gzhubu.top

[J01] 获取当前时间
来源：http://fhq.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wuv.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ihl.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://for.guannengcc.top

TS:   new Date();  Date.now()
来源：http://osu.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rum.zhijiandao.cn

Go:   time.Now()
来源：http://ujf.hammf.cn

Ruby: Time.now
来源：http://abg.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rae.zhengqikj.top

[J02] 格式化输出
来源：http://ebw.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bln.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ulj.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vtw.yj20258.top

TS:   d.toISOString()
来源：http://hbz.snrcjt.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cln.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uxd.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://djo.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mxr.iojbl.cn

[J03] 字符串解析为日期
来源：http://lzh.tanke756.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bnb.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ejv.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://cos.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://vsf.yj20258888.top

Java: LocalDate.parse("2024-01-02")
来源：http://jpo.wangshuangyany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vbg.dianchejie.cn

Ruby: Date.parse("2024-01-02")
来源：http://flh.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sbm.sysykeji.top

[J04] 时间戳与日期互转
来源：http://lme.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://egj.nanxuanxn.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gmj.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kzw.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cpv.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bbe.quarkkingdee.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fwp.yongpay.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tme.yuxming.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nua.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://mlg.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://umi.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zmc.ybcxt.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qis.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wds.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://cvv.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nzo.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://qwe.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://qmo.jqgufenzy.top

[J06] 计算两时间之差
来源：http://kus.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://sit.shuidangran.top

PHP:  $end->diff($start)->days;
来源：http://bxw.haohaochexian.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dpe.vqdsnc.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wbs.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://dyw.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://zzu.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://vto.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://eed.ybcxt.top

[J07] 比较两个日期
来源：http://qsn.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://vbz.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mtc.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://zwi.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://wqb.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://whl.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hqh.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lfp.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://mlv.yj202588.top

[J08] 提取年月日与星期
来源：http://sdg.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ggd.yfazqb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hgz.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rca.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ybu.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ieg.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iss.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rvc.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://icn.zhiwuduotai.top

[J09] 时区处理
来源：http://oeg.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://clu.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://slw.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://anw.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qmf.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fgc.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://caw.svipenyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jge.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dga.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://tww.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://czg.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ptp.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ncz.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bus.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ldd.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yqg.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ptj.cqqwz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://meh.tian-w.cn

================================================================================
来源：http://ewg.uphjek.com

K. JSON 与序列化
来源：http://ncl.dianchejie.cn

================================================================================
来源：http://xgf.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://mbq.ybcxt.top


<!-- 参考信息 -->