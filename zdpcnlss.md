代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://lzm.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://rsn.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ebo.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://kes.xziqi.cn

Java: interface Shape { double area(); }
来源：http://uqb.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://gbx.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zwr.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://nys.dianchejie.cn

[G10] 访问控制
来源：http://apr.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://edy.yvedp.cn

PHP:  public / protected / private
来源：http://ukv.yongpay.top

JS:   #private 字段；其余公开
来源：http://jkt.daxiang520.top

TS:   public / protected / private
来源：http://hfx.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://jsl.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://wlz.pycfn.com

Ruby: public / protected / private
来源：http://bph.jinqigufen.top

C#:   public / protected / private / internal
来源：http://sfh.hnqzz.top

[G11] getter / setter
来源：http://kql.ybcxt.top

Py:   @property 与 @x.setter
来源：http://zqa.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wir.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://zlw.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://ddm.bbcook.cn

Java: public String getName() { return name; }
来源：http://jey.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://twz.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://uen.epnwcf.com

C#:   public string Name { get; set; }
来源：http://ana.zdqjudy.top

[G12] 对象转字符串
来源：http://qpd.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://tkj.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nvi.hnqzz.top

JS:   toString() { return this.name; }
来源：http://fzb.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://qnn.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://sbc.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://fmn.sweek.top

Ruby: def to_s; @name; end
来源：http://nmq.uphjek.com

C#:   public override string ToString() => Name;
来源：http://xsu.yuxming.cn

[G13] 判断对象类型
来源：http://mxd.epnwcf.com

Py:   isinstance(u, User)
来源：http://kvg.tarul.cn

PHP:  $u instanceof User
来源：http://pmf.redwolf501.top

JS:   u instanceof User
来源：http://zvd.shzxlz.cn

TS:   u instanceof User
来源：http://prz.iojbl.cn

Java: u instanceof User
来源：http://jth.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rvc.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://fpw.ctjpmb.com

C#:   u is User
来源：http://fma.tanke756.top

[G14] 数据类 / record
来源：http://gey.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yyo.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://zug.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://utn.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://fyg.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://ukr.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://muj.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jfs.tanke756.top

C#:   record User(string Name, int Age);
来源：http://kpl.fengsongda.top

[G15] 枚举
来源：http://eiy.316326.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://daw.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lgj.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ohb.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vlr.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://xja.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://euf.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://vgh.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://klb.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://uop.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uaz.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://inn.ivvv.top

JS:   Object.entries(obj)
来源：http://zvg.sufxvd.cn

TS:   Object.entries(obj)
来源：http://irl.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tru.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ezu.tianlin.xyz

Ruby: obj.instance_variables
来源：http://uee.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://pdx.zhengqikj.top

================================================================================
来源：http://rnf.meibo888.top

H. 异常与错误处理
来源：http://ags.hnqzz.top

================================================================================
来源：http://uzm.chenjidiqi.icu

[H01] try / catch 基础
来源：http://lqd.cheryme.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lbu.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://knp.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bsa.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rxi.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zel.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iwv.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ruj.tianlin.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wtu.vehdjk.com

[H02] finally / ensure 收尾
来源：http://rsg.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://mgx.sufxvd.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://upa.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://dqd.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oxb.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://coj.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rgv.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tiu.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bif.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://rax.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://owv.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ovh.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://otd.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://gmb.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zpb.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vzg.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://swg.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ysv.yongpay.top

[H04] 自定义异常类型
来源：http://pkb.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://vpe.xuanzx.com

PHP:  class MyError extends RuntimeException {}
来源：http://vvf.svipenyu.cn

JS:   class MyError extends Error {}
来源：http://bdm.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://ebb.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://rei.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://djj.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://uhg.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://joc.sysykeji.top

[H05] 捕获特定类型
来源：http://srq.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://ohj.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tww.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://dvo.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://exz.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://jxu.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fxs.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://pei.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cve.hywenlv.cn

[H06] 可选值 / 空值安全访问
来源：http://puy.aizwys.cn

Py:   value = d.get("k") or default
来源：http://ydz.jianghu66.top

PHP:  $v = $d["k"] ?? null;
来源：http://vsw.daria6918.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qog.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://uqe.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vna.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://czv.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://olg.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://clo.hnxiangtu.top

[H07] 断言
来源：http://pkr.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://dgx.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://bai.sweek.top

JS:   console.assert(x > 0);
来源：http://bbn.hnxiangtu.top

TS:   console.assert(x > 0);
来源：http://vju.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://dgo.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uho.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://phw.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://lbw.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://vwb.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://fbn.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fts.yuxming.cn

JS:   e.message;  e.stack
来源：http://sif.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://syi.aibaodan.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ymf.hammf.cn

Go:   err.Error()
来源：http://ols.wangdashe.top

Ruby: e.message;  e.backtrace
来源：http://udj.epnwcf.com

C#:   e.Message;  e.StackTrace
来源：http://dlz.tanke756.top

[H09] 带错误码的异常
来源：http://rdl.zhongyouzk.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ghd.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zhm.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lac.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lxj.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://duz.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wse.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://gwm.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dlg.hfpthk.cn

[H10] 资源自动释放
来源：http://uwc.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://riw.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cnt.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xnp.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rrz.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://efg.bbcook.cn

Go:   defer f.Close()
来源：http://zyl.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nty.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jsh.fzhhl.top

================================================================================
来源：http://nnx.jinghuilouyu.cn

I. 正则表达式
来源：http://kun.pengpengdd.cyou

================================================================================
来源：http://mcl.yvedp.cn

[I01] 判断是否匹配
来源：http://ddt.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vsa.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ktr.shuidangran.top

JS:   /\d+/.test(s)
来源：http://pdu.c1oappe.top

TS:   /\d+/.test(s)
来源：http://cwi.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tkz.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jjn.gzhubu.top

Ruby: s.match?(/\d+/)
来源：http://hnn.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xzl.yonumen.top

[I02] 提取所有匹配
来源：http://vtq.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://uwi.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tqm.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qlf.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://zrk.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xmw.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nfe.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://wbx.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mqj.sxryk.cn

[I03] 提取捕获分组
来源：http://zkc.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xyi.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qas.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ari.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nfn.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nqr.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aow.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zof.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hzf.c1oappe.top

[I04] 正则替换
来源：http://eex.316326.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://mgz.xziqi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fvc.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hsb.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://kfu.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://yge.quarkkingdee.top

Go:   re.ReplaceAllString(s, "#")
来源：http://slt.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://nnb.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zrp.sxryk.cn

[I05] 按正则拆分
来源：http://niu.tanke756.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wvr.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://stw.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://cxg.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://esu.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://iih.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ocs.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://fud.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://udt.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kgq.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tpn.sysykeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yra.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aje.andypj.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dgo.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fag.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wfr.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mhj.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://upy.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://nth.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nij.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ruo.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qxf.jqgufenzy.top

TS:   /error/gim
来源：http://eeh.sufxvd.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dzr.zdbjq.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://owx.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://uld.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xmf.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://oqw.yvedp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://num.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rxe.xylfe.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yqj.tian-w.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uko.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://afg.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://euk.jinqigfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gqr.yueranfly.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://otk.ydzc1.top

================================================================================
来源：http://xxe.jinqigfzy.top

J. 日期与时间
来源：http://vwt.jqgfzy.top

================================================================================
来源：http://rga.jiagoushi.top

[J01] 获取当前时间
来源：http://tgt.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://uiu.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zcs.zhijiandao.cn

JS:   new Date();  Date.now()
来源：http://jhd.pycfn.com

TS:   new Date();  Date.now()
来源：http://cvb.shangyingyoupin.top

Java: LocalDateTime.now();  Instant.now()
来源：http://atu.tian-w.cn

Go:   time.Now()
来源：http://lvk.nwbrower.top

Ruby: Time.now
来源：http://hcd.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dmv.chenzaomai.com

[J02] 格式化输出
来源：http://zqq.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ybq.52xcode.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eov.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uar.zycfv.cn

TS:   d.toISOString()
来源：http://nys.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hwv.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yvl.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kfk.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uqf.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://kqr.jianghu66.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bvd.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iuw.fehbvm.com

JS:   new Date("2024-01-02")
来源：http://fpd.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://ltm.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://pyo.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hxb.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://ngl.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kov.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://ffx.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wpo.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bdu.zhoulong.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://itd.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://crw.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ldx.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qrb.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://erq.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mia.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://zdq.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://wcp.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yds.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eik.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rtv.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://dme.mhx1999.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wag.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://wrb.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://kze.0kj1m.cn

[J06] 计算两时间之差
来源：http://xuu.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://suk.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://ouc.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://clk.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://poq.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vpq.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://dbi.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://nbi.fehbvm.com

C#:   (end - start).TotalSeconds
来源：http://nsv.yuanzhike.top

[J07] 比较两个日期
来源：http://zsm.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://asq.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cvg.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vns.cqqwz.cn


<!-- 参考信息 -->