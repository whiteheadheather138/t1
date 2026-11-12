代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://fll.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xtv.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ovr.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://qwz.gzhubu.top

Java: interface Shape { double area(); }
来源：http://rxw.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://pmy.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uwv.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://lcy.zhaomingkeji.xyz

[G10] 访问控制
来源：http://uge.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://cxe.tanke756.top

PHP:  public / protected / private
来源：http://cdv.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://iud.andypj.xyz

TS:   public / protected / private
来源：http://mcf.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://mrw.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sjz.gzhubu.top

Ruby: public / protected / private
来源：http://sri.jianghu66.top

C#:   public / protected / private / internal
来源：http://qqw.uphjek.com

[G11] getter / setter
来源：http://wjp.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://twg.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kzi.sweek.top

JS:   get name() { return this._name; }
来源：http://hnz.ehwqpu.com

TS:   get name(): string { return this._name; }
来源：http://ovb.xinyue.icu

Java: public String getName() { return name; }
来源：http://xdk.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://peb.ybcxt.top

Ruby: attr_accessor :name
来源：http://yyw.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://psf.jianghu66.top

[G12] 对象转字符串
来源：http://neh.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://bke.uphjek.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://fab.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://hpq.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://ase.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://eqt.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dag.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://hip.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://ris.gzhubu.top

[G13] 判断对象类型
来源：http://oxi.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://daa.zdbjq.cn

PHP:  $u instanceof User
来源：http://ofr.yangfankeji.com

JS:   u instanceof User
来源：http://dpt.smart0.xyz

TS:   u instanceof User
来源：http://zis.52xcode.cn

Java: u instanceof User
来源：http://fre.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lus.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://yre.hammf.cn

C#:   u is User
来源：http://uwg.wangdashe.top

[G14] 数据类 / record
来源：http://ntu.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cvv.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://obo.cdnleiting.top

JS:   // 无内置：普通类或对象字面量
来源：http://csq.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://kfd.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://rrt.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://qyl.sjlbkw.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hyz.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://qzs.xuanzx.com

[G15] 枚举
来源：http://mro.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jjk.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rhj.9152youxi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hxx.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jib.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://mna.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nph.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://nyl.yueranfly.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://odc.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://pds.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jxa.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://mpy.cashguo.top

JS:   Object.entries(obj)
来源：http://jsw.jianghu66.top

TS:   Object.entries(obj)
来源：http://vdy.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lsz.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gco.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://kpc.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://khn.cdnleiting.top

================================================================================
来源：http://dun.gotoacloud.top

H. 异常与错误处理
来源：http://uxt.sufxvd.cn

================================================================================
来源：http://dbe.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://ilp.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mck.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qbe.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://moa.chenjidiqi.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://faf.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iyy.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://scq.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://urm.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hbx.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://fye.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://smc.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ata.chenlongwang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ibk.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lxq.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://baj.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://ztm.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uuw.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://skx.c1oappe.top

[H03] 主动抛出异常
来源：http://ygi.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://atc.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qyd.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://kri.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://pun.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://pwe.sysykeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yyt.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dqf.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://wgj.cucudq.cn

[H04] 自定义异常类型
来源：http://pkp.uphjek.com

Py:   class MyError(Exception): pass
来源：http://mwr.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://cct.redwolf501.top

JS:   class MyError extends Error {}
来源：http://qrz.zhijiandao.cn

TS:   class MyError extends Error {}
来源：http://ntw.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://qxr.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tft.mhx1999.top

Ruby: class MyError < StandardError; end
来源：http://uct.tarul.cn

C#:   class MyException : Exception {}
来源：http://xgz.vehdjk.com

[H05] 捕获特定类型
来源：http://abq.quarkkingdee.top

Py:   except ValueError as e:
来源：http://pzr.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ynu.ydjk.org.cn

JS:   if (e instanceof TypeError) {}
来源：http://caa.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://lah.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://gtd.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dwx.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://lpf.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://anw.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://hpn.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://xmy.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bkx.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://suk.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://hnu.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tah.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rmi.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://caq.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://kka.wangshuangyany.cn

[H07] 断言
来源：http://xea.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://rcz.daria6918.cn

PHP:  assert($x > 0);
来源：http://pax.hammf.cn

JS:   console.assert(x > 0);
来源：http://wya.birdmap.top

TS:   console.assert(x > 0);
来源：http://kcq.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://swg.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pds.kuanghao11.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vsh.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://cgf.52xcode.cn

[H08] 获取错误信息与堆栈
来源：http://pzi.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://jlh.jlsjyb.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hcb.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://wpi.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gnf.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sod.jinghuilouyu.cn

Go:   err.Error()
来源：http://ydi.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://wfv.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://xti.daria6918.cn

[H09] 带错误码的异常
来源：http://zfb.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tal.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kwf.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pkp.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ujk.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ifd.zhaomingkeji.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://siq.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://gld.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vhl.nanxuanxn.top

[H10] 资源自动释放
来源：http://nty.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sje.yj20258.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rmn.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xsr.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dqf.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://agb.jyoumei.cn

Go:   defer f.Close()
来源：http://uxc.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://apv.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://btd.ydzc1.top

================================================================================
来源：http://pzu.xylfe.cn

I. 正则表达式
来源：http://rza.aizwys.cn

================================================================================
来源：http://pbu.gaohongyu789.top

[I01] 判断是否匹配
来源：http://fmm.yfazqb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lzy.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cqf.uphjek.com

JS:   /\d+/.test(s)
来源：http://kgz.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://pkm.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bbz.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mlr.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://lvb.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://odx.jinqigufen.top

[I02] 提取所有匹配
来源：http://oru.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://ysa.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tqz.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://trt.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://oux.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vmw.nanxuanxn.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://apz.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://miq.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zwr.gotoacloud.top

[I03] 提取捕获分组
来源：http://nho.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wct.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nnn.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rjl.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jli.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://plx.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bfs.cashguo.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rhb.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nnx.ydzc1.top

[I04] 正则替换
来源：http://upm.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dba.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cpv.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://vyu.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://gak.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://sbd.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ykl.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mqv.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hjy.chenzaomai.com

[I05] 按正则拆分
来源：http://umj.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ozp.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://aoz.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://han.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://fsq.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://bjg.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sfl.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sun.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://juy.zhoulong.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dfd.zhijiandao.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kok.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zyy.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://obv.jiagoushi.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://syp.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uqk.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://scd.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://znr.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mwh.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://hnr.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://llh.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wiv.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iuu.hnxiangtu.top

TS:   /error/gim
来源：http://leq.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://okt.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kpw.dashuyun.cn

Ruby: s.scan(/error/i)
来源：http://rik.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bnp.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://tqf.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lib.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rjm.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qkv.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fyk.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vra.shangyingyoupin.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://glm.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eyr.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://efq.jyoumei.cn

================================================================================
来源：http://bly.cdnleiting.top

J. 日期与时间
来源：http://xqb.xylfe.cn

================================================================================
来源：http://pvh.fengsongda.top

[J01] 获取当前时间
来源：http://fnu.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://atc.gogol.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gpt.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://qib.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://ghn.sysykeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://teq.0kj1m.cn

Go:   time.Now()
来源：http://ulw.tian-w.cn

Ruby: Time.now
来源：http://bjw.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dlz.xuetiantiany.cn

[J02] 格式化输出
来源：http://lzv.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yde.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dqj.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zrc.haohaochexian.top

TS:   d.toISOString()
来源：http://aia.ehwqpu.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bhv.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zci.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dbv.zhiwuduotai.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cft.c1oappe.top

[J03] 字符串解析为日期
来源：http://kro.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://trw.zhaomingkeji.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ndi.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://fbk.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://bgo.yj20258.top

Java: LocalDate.parse("2024-01-02")
来源：http://krk.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xkg.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://nrb.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ehg.smart0.xyz

[J04] 时间戳与日期互转
来源：http://azg.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uta.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ujl.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pka.dianchejie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fpx.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vmo.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://paf.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uqz.zycfv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kqv.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://fqs.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://giv.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ntj.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jvi.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cvs.redwolf501.top

Java: LocalDate.now().plusDays(7)
来源：http://drf.ctjpmb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qwp.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://xvd.nanxuanxn.top

C#:   DateTime.Now.AddDays(7)
来源：http://kji.quarkkingdee.top

[J06] 计算两时间之差
来源：http://tcf.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://cmd.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://kgo.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://riy.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ilb.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://vdl.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://wtd.fengsongda.top

Ruby: end - start                 # 返回秒数
来源：http://qrh.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://pww.yongpay.top

[J07] 比较两个日期
来源：http://oow.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://fbb.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iyd.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://zjp.ivvv.top


<!-- 参考信息 -->