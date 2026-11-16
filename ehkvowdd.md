代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://zrx.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://rxo.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nux.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://rvp.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://mch.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://ten.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xpe.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://pyf.jinghuilouyu.cn

[G10] 访问控制
来源：http://qcn.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://ydd.ctjpmb.com

PHP:  public / protected / private
来源：http://hxy.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://niy.aizwys.cn

TS:   public / protected / private
来源：http://xnd.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://zdg.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://xva.sysykeji.top

Ruby: public / protected / private
来源：http://lst.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://kmh.sufxvd.cn

[G11] getter / setter
来源：http://iqc.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://jhp.vqdsnc.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gds.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://gus.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://vai.sweek.top

Java: public String getName() { return name; }
来源：http://ber.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://qcy.zhengqikj.top

Ruby: attr_accessor :name
来源：http://afn.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://qxt.zhengqikj.top

[G12] 对象转字符串
来源：http://ami.hywenlv.cn

Py:   def __str__(self): return self.name
来源：http://lvy.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://pvn.zhiwuduotai.top

JS:   toString() { return this.name; }
来源：http://jhf.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://oqb.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://mgf.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://kyw.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://tzl.dashuyun.cn

C#:   public override string ToString() => Name;
来源：http://pfa.daria6918.cn

[G13] 判断对象类型
来源：http://erb.cqqwz.cn

Py:   isinstance(u, User)
来源：http://fsg.andypj.xyz

PHP:  $u instanceof User
来源：http://kku.fanxiaobao.xyz

JS:   u instanceof User
来源：http://mwt.cdnleiting.top

TS:   u instanceof User
来源：http://znl.ehwqpu.com

Java: u instanceof User
来源：http://zap.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nvn.c1oappe.top

Ruby: u.is_a?(User)
来源：http://rwm.fzhhl.top

C#:   u is User
来源：http://uul.sysykeji.top

[G14] 数据类 / record
来源：http://jco.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tfs.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://zzw.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mza.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://quj.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://ujk.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://rxh.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jcp.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://dvm.pengpengdd.cyou

[G15] 枚举
来源：http://fhr.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vet.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rrp.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iyo.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dgg.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://vqe.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zql.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://dzd.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nma.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://voo.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qmx.tanke756.top

PHP:  get_object_vars($obj);
来源：http://mcp.ybcxt.top

JS:   Object.entries(obj)
来源：http://ybq.c1oappe.top

TS:   Object.entries(obj)
来源：http://xnf.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qwn.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://irk.hysaishi.cn

Ruby: obj.instance_variables
来源：http://npy.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://hwy.yanxiufei.cn

================================================================================
来源：http://mye.yonumen.top

H. 异常与错误处理
来源：http://omz.0kj1m.cn

================================================================================
来源：http://gnn.pycfn.com

[H01] try / catch 基础
来源：http://cqz.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hbf.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kos.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kjj.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rca.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iaz.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ioo.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://frf.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mxv.yuanzhike.top

[H02] finally / ensure 收尾
来源：http://ufi.ybcxt.top

Py:   try: f()⏎finally: cleanup()
来源：http://qhl.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kuv.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://chi.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ikg.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://vqh.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yrt.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://saw.xingfuxueyuan.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://hii.cheryme.top

[H03] 主动抛出异常
来源：http://gtr.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://vps.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ckq.316326.xyz

JS:   throw new Error("错误信息");
来源：http://wtj.pycfn.com

TS:   throw new Error("错误信息");
来源：http://owy.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dod.gotoacloud.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iko.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gal.zhaomingkeji.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://qem.guannengcc.top

[H04] 自定义异常类型
来源：http://rty.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://pse.jinyuanbaomall.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rvy.hesvh.cn

JS:   class MyError extends Error {}
来源：http://phc.iojbl.cn

TS:   class MyError extends Error {}
来源：http://tqs.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://stu.316326.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ezw.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://hwl.sysykeji.top

C#:   class MyException : Exception {}
来源：http://dwa.vqdsnc.cn

[H05] 捕获特定类型
来源：http://cls.zdbjq.cn

Py:   except ValueError as e:
来源：http://svu.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wje.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://apo.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://cgh.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://byj.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ttm.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://kwc.kuanghao11.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gzz.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://wtx.yfazqb.com

Py:   value = d.get("k") or default
来源：http://dzb.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qde.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://dsl.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://vob.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mkw.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bhh.gaohongyu789.top

Ruby: d&.dig(:a, :b)
来源：http://rqf.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://ufs.ppjwa.cn

[H07] 断言
来源：http://tbs.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://raz.yonumen.top

PHP:  assert($x > 0);
来源：http://zsq.andypj.xyz

JS:   console.assert(x > 0);
来源：http://ciu.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://sbi.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://psw.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dzi.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://zdy.zhoulong.xyz

C#:   Debug.Assert(x > 0);
来源：http://jxo.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://ovf.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://nos.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cdi.sxryk.cn

JS:   e.message;  e.stack
来源：http://dfb.pengpengdd.cyou

TS:   e instanceof Error ? e.message : String(e)
来源：http://mgw.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ljk.sjlbkw.cn

Go:   err.Error()
来源：http://ezu.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://urc.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://rvu.316326.xyz

[H09] 带错误码的异常
来源：http://lcg.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fdf.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yfk.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eqi.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iep.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mno.yj20258888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oua.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://dqk.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://eii.zhengqikj.top

[H10] 资源自动释放
来源：http://eeh.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mwf.hcnkem.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gqs.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://exj.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pqm.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fgz.0kj1m.cn

Go:   defer f.Close()
来源：http://gxo.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://brw.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vrx.redwolf501.top

================================================================================
来源：http://fwg.cucudq.cn

I. 正则表达式
来源：http://eka.316326.xyz

================================================================================
来源：http://rug.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://uev.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zjz.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://qee.uphjek.com

JS:   /\d+/.test(s)
来源：http://fgc.cucudq.cn

TS:   /\d+/.test(s)
来源：http://gpk.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jjk.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://syn.yj20258.top

Ruby: s.match?(/\d+/)
来源：http://olg.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bhu.guannengcc.top

[I02] 提取所有匹配
来源：http://ecf.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://zbc.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pdd.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fqi.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://wqk.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qni.tarul.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://izn.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://pic.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://toc.ybcxt.top

[I03] 提取捕获分组
来源：http://ani.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://skj.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hzm.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ktr.zycfv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lsj.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eht.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://otw.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vbj.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://far.uphjek.com

[I04] 正则替换
来源：http://iqe.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tvf.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qqr.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://udz.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://gby.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://wkn.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iyo.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tjs.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wdq.yvedp.cn

[I05] 按正则拆分
来源：http://xbb.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gjv.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lpv.ywan-chungtsiang.top

JS:   s.split(/\s*,\s*/)
来源：http://gsq.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://mfg.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://myc.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ooc.gzhubu.top

Ruby: s.split(/\s*,\s*/)
来源：http://hfo.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jaj.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hts.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sae.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cgk.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://trg.xuanzx.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kza.cashguo.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sry.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xrw.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gco.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://giy.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://pcu.jqgfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cae.tianlin.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ywb.guannengcc.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dwu.zhongyouzk.top

TS:   /error/gim
来源：http://zds.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bgy.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://utf.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://dwj.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dcw.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://xfc.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pny.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nuz.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://emt.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvq.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gof.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sgt.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fcy.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qln.zdqjudy.top

================================================================================
来源：http://qbr.chenlongwang.top

J. 日期与时间
来源：http://irp.shzxlz.cn

================================================================================
来源：http://qal.bbcook.cn

[J01] 获取当前时间
来源：http://hhd.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://opq.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nsh.ctjpmb.com

JS:   new Date();  Date.now()
来源：http://owr.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://vgc.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hvl.dashuyun.cn

Go:   time.Now()
来源：http://xcx.svipenyu.cn

Ruby: Time.now
来源：http://nlx.tianlin.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sjn.yfazqb.com

[J02] 格式化输出
来源：http://xjs.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zod.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zft.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zag.jianghu66.top

TS:   d.toISOString()
来源：http://ddd.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dsi.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xor.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://des.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ndp.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://dvl.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vyz.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eqi.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://ntc.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://kpp.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wlx.dianchejie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vad.fktsv.cn

Ruby: Date.parse("2024-01-02")
来源：http://xhy.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rwm.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://uzl.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jvm.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eri.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qvt.fzhhl.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gpl.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://noi.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cgu.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tmu.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ytg.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://qoe.316326.xyz

Py:   now + timedelta(days=7)
来源：http://mwf.sxryk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rpz.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bgm.xziqi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xut.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://ckx.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://flb.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://svs.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://luc.ehwqpu.com

[J06] 计算两时间之差
来源：http://zjx.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://ivx.chenzaomai.com

PHP:  $end->diff($start)->days;
来源：http://nbf.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xin.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lqm.jyoumei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hty.uphjek.com

Go:   end.Sub(start).Hours()
来源：http://khd.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://aty.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://tzw.andypj.xyz

[J07] 比较两个日期
来源：http://uwi.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://zey.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qpd.shanyushiyangtech.top

JS:   d1.getTime() < d2.getTime()
来源：http://dao.jianghu66.top


<!-- 参考信息 -->