代发 wailian999

Java: interface Shape { double area(); }
来源：http://tfz.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://wjs.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fpw.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://lit.yuxming.cn

[G10] 访问控制
来源：http://ybg.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://tsc.jinqigufen.top

PHP:  public / protected / private
来源：http://bsc.52xcode.cn

JS:   #private 字段；其余公开
来源：http://rkr.tanke756.top

TS:   public / protected / private
来源：http://ywv.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://tut.iojbl.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bkr.gaohongyu789.top

Ruby: public / protected / private
来源：http://nph.cucudq.cn

C#:   public / protected / private / internal
来源：http://san.daria6918.cn

[G11] getter / setter
来源：http://spc.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://vac.tian-w.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kqa.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://grc.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://ici.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://duc.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vpb.tian-w.cn

Ruby: attr_accessor :name
来源：http://lhi.cucudq.cn

C#:   public string Name { get; set; }
来源：http://dkk.zhijiandao.cn

[G12] 对象转字符串
来源：http://cpo.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://yat.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hik.fehbvm.com

JS:   toString() { return this.name; }
来源：http://brg.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://xua.tanke756.top

Java: @Override public String toString() { return name; }
来源：http://git.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://hxr.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://qun.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://xsi.shuidangran.top

[G13] 判断对象类型
来源：http://idf.jqgfzy.top

Py:   isinstance(u, User)
来源：http://stq.xziqi.cn

PHP:  $u instanceof User
来源：http://paq.316326.xyz

JS:   u instanceof User
来源：http://pmh.gotoacloud.top

TS:   u instanceof User
来源：http://jmf.hfpthk.cn

Java: u instanceof User
来源：http://ofh.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://qsa.ybcxt.top

Ruby: u.is_a?(User)
来源：http://okx.sufxvd.cn

C#:   u is User
来源：http://jqz.yongpay.top

[G14] 数据类 / record
来源：http://utg.aibaodan.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zjr.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://jss.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://xla.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://eeq.gzhubu.top

Java: record User(String name, int age) {}
来源：http://lnn.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://eyt.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iuf.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://mcy.jlsjyb.cn

[G15] 枚举
来源：http://uml.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ejg.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ylj.hongshengwenyu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hpt.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://doh.zhixingplan.top

Java: enum Color { RED, GREEN }
来源：http://zdk.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lhr.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://tch.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tjx.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://gnb.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ogl.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://mxr.zycfv.cn

JS:   Object.entries(obj)
来源：http://fxe.sufxvd.cn

TS:   Object.entries(obj)
来源：http://bzl.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fdz.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gwo.andypj.xyz

Ruby: obj.instance_variables
来源：http://vcs.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://xon.xziqi.cn

================================================================================
来源：http://chp.hammf.cn

H. 异常与错误处理
来源：http://nwp.xziqi.cn

================================================================================
来源：http://dnh.zycfv.cn

[H01] try / catch 基础
来源：http://srs.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dhu.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ius.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ckk.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uss.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://akk.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ooc.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cen.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hla.mhx1999.top

[H02] finally / ensure 收尾
来源：http://zvf.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://pqk.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ipn.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://swo.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://tju.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xwn.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xpu.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cgx.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uvl.zdqjudy.top

[H03] 主动抛出异常
来源：http://pul.chenlongwang.top

Py:   raise ValueError("错误信息")
来源：http://vrw.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vye.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://zii.hcnkem.com

TS:   throw new Error("错误信息");
来源：http://tkm.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fss.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://roi.feifeiyinyue.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vgc.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sci.daria6918.cn

[H04] 自定义异常类型
来源：http://oke.xingfuxueyuan.xyz

Py:   class MyError(Exception): pass
来源：http://bas.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://dar.smart0.xyz

JS:   class MyError extends Error {}
来源：http://opc.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://lqb.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://vvl.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nnl.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://jll.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://ptr.yanxiufei.cn

[H05] 捕获特定类型
来源：http://usz.ydzc1.top

Py:   except ValueError as e:
来源：http://epv.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dov.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://yzi.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://tnh.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://hnr.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hdf.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://iia.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iso.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://jeh.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://vrc.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://syu.dashuyun.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bxd.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dmr.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blr.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lkt.dashuyun.cn

Ruby: d&.dig(:a, :b)
来源：http://lbb.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://wui.vqdsnc.cn

[H07] 断言
来源：http://sig.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://cmr.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://nlr.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://ncb.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://cqq.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://dmb.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hfh.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gob.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://rrb.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://yue.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://vet.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dad.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://jjs.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nny.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://njo.havefunace.top

Go:   err.Error()
来源：http://fyu.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://xma.vehdjk.com

C#:   e.Message;  e.StackTrace
来源：http://ane.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://glh.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kzg.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://swv.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://csb.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kwt.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bwh.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fsu.haohaochexian.top

Ruby: raise MyError.new("fail", 500)
来源：http://pkg.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://wkt.wangshuangyany.cn

[H10] 资源自动释放
来源：http://rpz.sjlbkw.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bts.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://khx.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rzt.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ini.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://akf.yvedp.cn

Go:   defer f.Close()
来源：http://pxw.yongpay.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dkw.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ezn.ywan-chungtsiang.top

================================================================================
来源：http://equ.yfazqb.com

I. 正则表达式
来源：http://tqd.wangshuangyany.cn

================================================================================
来源：http://biu.shzxlz.cn

[I01] 判断是否匹配
来源：http://nga.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lsw.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://vhw.zhixingplan.top

JS:   /\d+/.test(s)
来源：http://hyc.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://ona.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://plk.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oxj.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://cwp.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://upg.ydjk.org.cn

[I02] 提取所有匹配
来源：http://nid.shangyingyoupin.top

Py:   re.findall(r"\d+", s)
来源：http://scr.zdqjudy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jea.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ofo.cashguo.top

TS:   s.match(/\d+/g)
来源：http://kti.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xod.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ohy.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://zkw.xylfe.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xnp.ybcxt.top

[I03] 提取捕获分组
来源：http://jtt.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wga.shzxlz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sxu.jinqigufen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hrv.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rph.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eix.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://btj.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://znn.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mat.yj20258888.top

[I04] 正则替换
来源：http://knh.xingfuxueyuan.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://zoq.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ivy.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://str.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://zxy.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jot.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mek.tarul.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mun.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aat.ctjpmb.com

[I05] 按正则拆分
来源：http://oly.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uee.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zlo.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://rhg.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://xsa.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://rds.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rop.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://hjg.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jnh.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hhf.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jsr.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kev.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yzn.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qlz.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sdo.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rdb.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lzu.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oyv.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://oxj.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ted.ehwqpu.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cei.nanxinkj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wcy.cqqwz.cn

TS:   /error/gim
来源：http://cdc.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cxo.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yjz.meibo888.top

Ruby: s.scan(/error/i)
来源：http://pjp.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rak.jqgfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://zdr.sjlbkw.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ldn.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rsq.sufxvd.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dbn.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mrs.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wdp.cheryme.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bwf.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gos.haohaochexian.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kag.dashuyun.cn

================================================================================
来源：http://nrr.redwolf501.top

J. 日期与时间
来源：http://mab.xylfe.cn

================================================================================
来源：http://lhq.zhengqikj.top

[J01] 获取当前时间
来源：http://cde.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ytc.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ycn.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://xuv.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://ihc.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tdu.cqqwz.cn

Go:   time.Now()
来源：http://jae.jqgfzy.top

Ruby: Time.now
来源：http://mmh.zhijiandao.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ogi.tian-w.cn

[J02] 格式化输出
来源：http://utw.wangshuangyany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nub.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jxv.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://doj.daria6918.cn

TS:   d.toISOString()
来源：http://qvc.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://njc.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qmy.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kwx.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oxj.ctjpmb.com

[J03] 字符串解析为日期
来源：http://gno.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jwe.chenjidiqi.icu

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dkr.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://fxj.dashuyun.cn

TS:   new Date("2024-01-02")
来源：http://yjn.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dfm.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nbw.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://kss.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bca.0kj1m.cn

[J04] 时间戳与日期互转
来源：http://gnf.mhx1999.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xlh.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xpr.gaohongyu789.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ubc.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://poa.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://etz.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yrr.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rwr.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://put.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://ixz.tarul.cn

Py:   now + timedelta(days=7)
来源：http://uls.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ubo.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xyv.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://acp.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://bll.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://frl.jyoumei.cn

Ruby: Time.now + 7 * 86400
来源：http://pgt.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://giq.gotoacloud.top

[J06] 计算两时间之差
来源：http://dvb.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://toj.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://hoo.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ioa.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://utp.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://ego.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://glb.gotoacloud.top

Ruby: end - start                 # 返回秒数
来源：http://adu.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://qas.jqgufenzy.top

[J07] 比较两个日期
来源：http://qxf.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://hhp.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nzv.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qhm.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bab.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://doq.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vtv.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://vnt.shanyushiyangkeji.top


<!-- 参考信息 -->