代发 wailian999

TS:   public / protected / private
来源：http://iuw.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://tcg.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://eho.shuidangran.top

Ruby: public / protected / private
来源：http://slm.smart0.xyz

C#:   public / protected / private / internal
来源：http://weq.tanke756.top

[G11] getter / setter
来源：http://roa.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://nsl.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ywb.redwolf501.top

JS:   get name() { return this._name; }
来源：http://yqq.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://ifz.gogol.net.cn

Java: public String getName() { return name; }
来源：http://evr.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lzt.yvedp.cn

Ruby: attr_accessor :name
来源：http://boj.fehbvm.com

C#:   public string Name { get; set; }
来源：http://xfu.daxiang520.top

[G12] 对象转字符串
来源：http://ewu.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://gix.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://fyx.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://xgo.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://rnt.andypj.xyz

Java: @Override public String toString() { return name; }
来源：http://jdo.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://hon.tarul.cn

Ruby: def to_s; @name; end
来源：http://uze.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://rrx.svipenyu.cn

[G13] 判断对象类型
来源：http://jwl.epnwcf.com

Py:   isinstance(u, User)
来源：http://vpq.yongpay.top

PHP:  $u instanceof User
来源：http://hjv.316326.xyz

JS:   u instanceof User
来源：http://bqg.ehwqpu.com

TS:   u instanceof User
来源：http://zvl.shanyushiyangtech.top

Java: u instanceof User
来源：http://cmx.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dhx.hesvh.cn

Ruby: u.is_a?(User)
来源：http://csf.haohaochexian.top

C#:   u is User
来源：http://oog.uphjek.com

[G14] 数据类 / record
来源：http://xiw.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cek.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://ghq.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://qgj.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://pds.pycfn.com

Java: record User(String name, int age) {}
来源：http://uxf.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://krv.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mbn.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://nzu.hysaishi.cn

[G15] 枚举
来源：http://pke.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mbl.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tpr.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lam.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bcg.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://bsc.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lxs.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://njh.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mgg.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://gcc.snrcjt.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hrt.uphjek.com

PHP:  get_object_vars($obj);
来源：http://adp.xuanzx.com

JS:   Object.entries(obj)
来源：http://xks.gogol.net.cn

TS:   Object.entries(obj)
来源：http://utd.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nmw.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wdy.xuanzx.com

Ruby: obj.instance_variables
来源：http://rpb.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://fan.yuanzhike.top

================================================================================
来源：http://gkf.tanke756.top

H. 异常与错误处理
来源：http://ccp.xingfuxueyuan.xyz

================================================================================
来源：http://lja.jqgfzy.top

[H01] try / catch 基础
来源：http://jaf.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wev.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://epm.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vdi.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ntc.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qwx.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ysb.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yfm.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gsu.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://uvl.hongshengwenyu.top

Py:   try: f()⏎finally: cleanup()
来源：http://iho.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dby.pycfn.com

JS:   try { f(); } finally { cleanup(); }
来源：http://lnf.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uai.cheryme.top

Java: try { f(); } finally { cleanup(); }
来源：http://reh.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qgm.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vwi.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eaf.xziqi.cn

[H03] 主动抛出异常
来源：http://gzh.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://eqi.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://omp.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://yue.zhengqikj.top

TS:   throw new Error("错误信息");
来源：http://dia.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://had.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://emo.zycfv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jxj.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qif.xinyue.icu

[H04] 自定义异常类型
来源：http://oii.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://ptj.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://lwr.xziqi.cn

JS:   class MyError extends Error {}
来源：http://ixm.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://ywl.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://rbm.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qja.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://spi.hcnkem.com

C#:   class MyException : Exception {}
来源：http://sfr.ydjk.org.cn

[H05] 捕获特定类型
来源：http://mbi.uphjek.com

Py:   except ValueError as e:
来源：http://jgb.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xbn.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://gyt.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://dqv.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://uoy.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oqv.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://bsg.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://icn.cheryme.top

[H06] 可选值 / 空值安全访问
来源：http://sqx.yonumen.top

Py:   value = d.get("k") or default
来源：http://rhr.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qjx.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://mtp.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ixw.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zcu.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eci.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://mwk.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://wps.sysykeji.top

[H07] 断言
来源：http://fbn.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://evw.wangdashe.top

PHP:  assert($x > 0);
来源：http://ekg.chenlongwang.top

JS:   console.assert(x > 0);
来源：http://ezp.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://dsz.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://ucd.yj202588.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lcv.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wps.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://cmi.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://nqz.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://mmi.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ake.iojbl.cn

JS:   e.message;  e.stack
来源：http://fif.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://lvh.jlsjyb.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rwa.cashguo.top

Go:   err.Error()
来源：http://xsn.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://mby.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://vgd.birdmap.top

[H09] 带错误码的异常
来源：http://nec.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nrn.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ysa.yonumen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lmt.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hfz.yj20258.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://esr.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wdo.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://dsc.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cfm.ctjpmb.com

[H10] 资源自动释放
来源：http://lje.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gon.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yrv.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mwf.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cno.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kus.pengpengdd.cyou

Go:   defer f.Close()
来源：http://kkl.smart0.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lfi.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bnq.smart0.xyz

================================================================================
来源：http://shq.jianghu66.top

I. 正则表达式
来源：http://yxf.yanxiufei.cn

================================================================================
来源：http://gdn.feifeiyinyue.top

[I01] 判断是否匹配
来源：http://orf.cucudq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sjr.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://rfx.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://vfk.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://nfj.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hnb.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zte.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://knl.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ohg.tarul.cn

[I02] 提取所有匹配
来源：http://nil.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://civ.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gdl.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cdd.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://ywj.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xlk.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vzd.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://wza.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xis.birdmap.top

[I03] 提取捕获分组
来源：http://ipz.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yde.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mwb.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vik.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oow.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oyr.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://emg.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hzz.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wyt.hfpthk.cn

[I04] 正则替换
来源：http://jps.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zss.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fcg.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://cdg.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://org.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://ayo.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://jfp.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pei.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://twx.zdqjudy.top

[I05] 按正则拆分
来源：http://wii.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://usi.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kfk.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://sod.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://ait.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://vfk.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zmj.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ajv.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qro.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gzg.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sbn.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kjo.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqj.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sko.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://avm.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sax.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fch.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://azg.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://pux.hcnkem.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wmc.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://igo.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uqt.jinqigfzy.top

TS:   /error/gim
来源：http://eis.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tqi.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yew.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://lir.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cnk.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://txf.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lpf.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bal.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fwt.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mcx.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://let.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lqw.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://okj.ydjk.org.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dpt.kuanghao11.cn

================================================================================
来源：http://rck.9152youxi.cn

J. 日期与时间
来源：http://jqk.snrcjt.cn

================================================================================
来源：http://cwu.ydjk.org.cn

[J01] 获取当前时间
来源：http://gsr.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://rfs.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vpk.mhx1999.top

JS:   new Date();  Date.now()
来源：http://qan.redwolf501.top

TS:   new Date();  Date.now()
来源：http://xvh.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nib.aizwys.cn

Go:   time.Now()
来源：http://iaq.jiagoushi.top

Ruby: Time.now
来源：http://hdm.316326.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dhm.tian-w.cn

[J02] 格式化输出
来源：http://fnh.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uxe.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mky.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zpu.haohaochexian.top

TS:   d.toISOString()
来源：http://ilr.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cnw.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pur.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxb.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://feu.havefunace.top

[J03] 字符串解析为日期
来源：http://val.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nbt.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xxi.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://zuq.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://apd.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://zgv.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wty.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://jkn.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://olo.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://odb.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bir.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aft.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nii.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nzb.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pzx.gogol.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://keq.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rhs.fanxiaobao.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fhc.0kj1m.cn

[J05] 时间加减（加 7 天）
来源：http://gel.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://grg.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pho.gotoacloud.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vsw.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dbt.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://fiy.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wfp.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://afu.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kqf.sxryk.cn

[J06] 计算两时间之差
来源：http://euc.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://yvz.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://szx.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://web.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tfe.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://fxe.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://esj.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://png.wangdashe.top

C#:   (end - start).TotalSeconds
来源：http://nxk.uphjek.com

[J07] 比较两个日期
来源：http://pwc.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://alx.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://erm.cqqwz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sjj.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fbk.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://owe.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ttz.0kj1m.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ykv.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://npv.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://goa.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kjv.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://akt.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://glm.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gnj.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jub.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nnw.zhengqikj.top


<!-- 参考信息 -->