代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://ffw.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://ocl.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://fpq.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://eqd.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://ovn.xylfe.cn

Ruby: def to_s; @name; end
来源：http://vul.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://kew.aibaodan.cn

[G13] 判断对象类型
来源：http://jgp.316326.xyz

Py:   isinstance(u, User)
来源：http://jyo.smart0.xyz

PHP:  $u instanceof User
来源：http://sgk.yj202588.top

JS:   u instanceof User
来源：http://adc.dashuyun.cn

TS:   u instanceof User
来源：http://nwc.zhijiandao.cn

Java: u instanceof User
来源：http://hbm.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yix.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://zeg.quarkkingdee.top

C#:   u is User
来源：http://rwb.0kj1m.cn

[G14] 数据类 / record
来源：http://vnq.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gkm.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://tml.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://dpv.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://ols.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://cel.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://zws.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://utg.ivvv.top

C#:   record User(string Name, int Age);
来源：http://lbs.fehbvm.com

[G15] 枚举
来源：http://sxl.nwbrower.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bjh.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wni.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ecb.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://neb.sweek.top

Java: enum Color { RED, GREEN }
来源：http://cks.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wgt.ywan-chungtsiang.top

Ruby: Color = %i[red green].freeze
来源：http://nbk.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://egw.cashguo.top

[G16] 对象转数组 / 字典
来源：http://qyt.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jqb.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://pea.ydzc1.top

JS:   Object.entries(obj)
来源：http://gtb.hywenlv.cn

TS:   Object.entries(obj)
来源：http://pxm.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vjz.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://jfh.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://pkd.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://ewy.jinghuilouyu.cn

================================================================================
来源：http://whh.ydjk.org.cn

H. 异常与错误处理
来源：http://mqw.shanyushiyangkeji.top

================================================================================
来源：http://wmr.fktsv.cn

[H01] try / catch 基础
来源：http://sti.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dou.sufxvd.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vfo.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qkn.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bkq.yvedp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ksr.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ela.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tov.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lxx.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://quk.shanyushiyangtech.top

Py:   try: f()⏎finally: cleanup()
来源：http://lsj.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://orc.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://nra.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fkw.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://dca.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://chi.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pdd.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://nlb.52xcode.cn

[H03] 主动抛出异常
来源：http://qaf.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://qvs.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ebd.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://bsd.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://ipx.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gbu.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ssl.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xqh.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mra.wangdashe.top

[H04] 自定义异常类型
来源：http://pah.ivvv.top

Py:   class MyError(Exception): pass
来源：http://cvq.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://qrc.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://pus.epnwcf.com

TS:   class MyError extends Error {}
来源：http://vgm.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://itp.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zsn.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://ami.fzhhl.top

C#:   class MyException : Exception {}
来源：http://fsq.iojbl.cn

[H05] 捕获特定类型
来源：http://udi.ydjk.org.cn

Py:   except ValueError as e:
来源：http://zry.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uzq.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://zwu.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://sxk.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://uve.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fwy.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://aha.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ccf.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://nwd.bjfxy.top

Py:   value = d.get("k") or default
来源：http://tyu.52xcode.cn

PHP:  $v = $d["k"] ?? null;
来源：http://inj.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://xvv.yj20258.top

TS:   obj?.a?.b;  d ?? default
来源：http://ark.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://txn.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://cgv.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://adg.hnqzz.top

C#:   obj?.A?.B ?? default
来源：http://uuj.chenzaomai.com

[H07] 断言
来源：http://plc.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://koc.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://sdt.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://jvq.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://mzj.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://fnn.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://swe.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://daq.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://wtd.zhoulong.xyz

[H08] 获取错误信息与堆栈
来源：http://zfa.sweek.top

Py:   str(e);  traceback.format_exc()
来源：http://ykn.fktsv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vvx.jyoumei.cn

JS:   e.message;  e.stack
来源：http://jkl.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kly.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rwl.fktsv.cn

Go:   err.Error()
来源：http://jnh.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://aes.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://ode.pycfn.com

[H09] 带错误码的异常
来源：http://qoa.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mrc.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zfo.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ukv.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vmc.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ikp.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://erq.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://wdv.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qjd.tianlin.xyz

[H10] 资源自动释放
来源：http://djd.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://oxe.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://abr.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kqe.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://znr.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xln.pycfn.com

Go:   defer f.Close()
来源：http://gsi.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jed.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://smm.sufxvd.cn

================================================================================
来源：http://beh.kuanghao11.cn

I. 正则表达式
来源：http://diz.jinqigfzy.top

================================================================================
来源：http://lyz.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://khz.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://axj.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tuf.c1oappe.top

JS:   /\d+/.test(s)
来源：http://nii.jianghu66.top

TS:   /\d+/.test(s)
来源：http://mfb.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cfn.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qmn.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://aap.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hwe.smart0.xyz

[I02] 提取所有匹配
来源：http://qeh.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://mjs.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rox.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cxw.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://txm.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zbm.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://not.xinyue.icu

Ruby: s.scan(/\d+/)
来源：http://xvj.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uxu.jinqigufen.top

[I03] 提取捕获分组
来源：http://zeo.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://too.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mrk.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jdk.sxryk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mey.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ilt.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ckm.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iuh.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ckd.gzhubu.top

[I04] 正则替换
来源：http://mea.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yjn.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://otw.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wkl.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://rvr.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://sut.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://scu.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vga.bjfxy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dqd.shzxlz.cn

[I05] 按正则拆分
来源：http://qnc.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tzs.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mzu.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://xcw.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://wpk.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://fks.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ttk.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bik.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qtv.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lys.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jli.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fjv.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mxt.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dgj.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jnx.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://idu.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ugc.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zer.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://fah.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ygx.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://umq.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nrm.hysaishi.cn

TS:   /error/gim
来源：http://qnn.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yyc.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pub.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://ymf.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ixl.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://moz.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://odr.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zda.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ldd.feifeiyinyue.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://chn.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://psv.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bkt.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tsv.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://guh.yongpay.top

================================================================================
来源：http://dae.kuanghao11.cn

J. 日期与时间
来源：http://rsm.shanyushiyangtech.top

================================================================================
来源：http://srk.sjlbkw.cn

[J01] 获取当前时间
来源：http://qth.yuanzhike.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://syp.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://emp.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://oeo.aizwys.cn

TS:   new Date();  Date.now()
来源：http://wfe.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hyc.hywenlv.cn

Go:   time.Now()
来源：http://fwd.yangfankeji.com

Ruby: Time.now
来源：http://wtm.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zsg.ydjk.org.cn

[J02] 格式化输出
来源：http://qnf.tianlin.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dyj.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ypq.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ehb.yfazqb.com

TS:   d.toISOString()
来源：http://ovz.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iau.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zyx.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oey.hysaishi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nmr.cheryme.top

[J03] 字符串解析为日期
来源：http://ipl.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yto.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rsh.cheryme.top

JS:   new Date("2024-01-02")
来源：http://bgg.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://mxm.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ojj.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bmp.hnxiangtu.top

Ruby: Date.parse("2024-01-02")
来源：http://gye.pengpengdd.cyou

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sgx.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://fkj.zhengqikj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gbe.epnwcf.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lwe.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xnh.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://php.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rrw.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gwg.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qro.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kea.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://qfq.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://dzi.c1oappe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://fla.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://quf.fanxiaobao.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://irt.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://wbf.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uwr.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://ebz.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bap.hesvh.cn

[J06] 计算两时间之差
来源：http://ens.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://ryw.sweek.top

PHP:  $end->diff($start)->days;
来源：http://ixc.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ywc.ydjk.org.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cph.gzhubu.top

Java: Duration.between(start, end).toSeconds()
来源：http://fip.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://rqv.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://vey.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://jwd.jqgufenzy.top

[J07] 比较两个日期
来源：http://hhj.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://pbl.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pyg.mhx1999.top

JS:   d1.getTime() < d2.getTime()
来源：http://ptk.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://hmd.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://khn.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bnp.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://lou.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://hpw.hesvh.cn

[J08] 提取年月日与星期
来源：http://ogc.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qhz.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uex.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xlm.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vcg.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xqi.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nhl.ydzc1.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wsf.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://emd.0kj1m.cn

[J09] 时区处理
来源：http://jsl.yongpay.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uvb.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kce.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://djd.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wxg.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xcf.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://acb.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://syr.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zfe.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://tud.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://srb.wangshuangyany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ntg.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qzz.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eiz.jinyuanbaomall.cn


<!-- 参考信息 -->