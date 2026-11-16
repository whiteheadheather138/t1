代发 wailian999

[G10] 访问控制
来源：http://xsf.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://kvq.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://rnm.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://qqh.jyoumei.cn

TS:   public / protected / private
来源：http://alu.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://zgp.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://hmm.fehbvm.com

Ruby: public / protected / private
来源：http://vwx.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://hbo.guowangkeji.top

[G11] getter / setter
来源：http://tjg.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://ckb.shanyushiyangtech.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sek.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://dqf.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://ofb.ctjpmb.com

Java: public String getName() { return name; }
来源：http://hbi.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://qog.guowangkeji.top

Ruby: attr_accessor :name
来源：http://vwl.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://ndy.zycfv.cn

[G12] 对象转字符串
来源：http://nkx.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://yoz.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ecc.havefunace.top

JS:   toString() { return this.name; }
来源：http://slr.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://ybx.jqgfzy.top

Java: @Override public String toString() { return name; }
来源：http://dkt.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://hqc.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://iii.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://wuk.ydjk.org.cn

[G13] 判断对象类型
来源：http://ngc.meibo888.top

Py:   isinstance(u, User)
来源：http://xjh.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://xot.gogol.net.cn

JS:   u instanceof User
来源：http://wel.shuidangran.top

TS:   u instanceof User
来源：http://lux.xylfe.cn

Java: u instanceof User
来源：http://uge.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vml.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://tie.havefunace.top

C#:   u is User
来源：http://guz.chenjidiqi.icu

[G14] 数据类 / record
来源：http://imc.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://atb.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://gna.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://guf.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://lzk.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://neh.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://ydz.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mwq.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://vhb.dianchejie.cn

[G15] 枚举
来源：http://esq.hesvh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zvw.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://swd.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lur.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://myb.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://fcx.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://coh.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://yow.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://adf.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://yhl.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rnf.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://tkc.jinqigufen.top

JS:   Object.entries(obj)
来源：http://sjj.svipenyu.cn

TS:   Object.entries(obj)
来源：http://qfk.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jzf.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iuw.chenzaomai.com

Ruby: obj.instance_variables
来源：http://tyk.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://mwe.ybcxt.top

================================================================================
来源：http://ksa.epnwcf.com

H. 异常与错误处理
来源：http://irz.hesvh.cn

================================================================================
来源：http://kvg.sufxvd.cn

[H01] try / catch 基础
来源：http://nyy.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yyj.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bxy.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fdn.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qqa.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yxg.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zdh.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://slz.hfpthk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gvy.nwbrower.top

[H02] finally / ensure 收尾
来源：http://zcr.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://mnw.ehwqpu.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://uqm.yueranfly.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yva.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jpi.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://bam.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kiq.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://obp.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bpf.birdmap.top

[H03] 主动抛出异常
来源：http://rdf.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://lfz.sjlbkw.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wgd.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://xvd.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://ddg.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pdl.vqdsnc.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pow.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://daz.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ejq.ywan-chungtsiang.top

[H04] 自定义异常类型
来源：http://fql.cashguo.top

Py:   class MyError(Exception): pass
来源：http://bbd.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://fti.tanke756.top

JS:   class MyError extends Error {}
来源：http://mce.cucudq.cn

TS:   class MyError extends Error {}
来源：http://edm.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://arj.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hsw.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://gjt.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://pfz.zhoulong.xyz

[H05] 捕获特定类型
来源：http://xry.tianlin.xyz

Py:   except ValueError as e:
来源：http://abf.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://add.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://xgv.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://xjw.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://uxi.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hxc.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://ddv.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xve.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://pjr.yueranfly.top

Py:   value = d.get("k") or default
来源：http://nxp.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hlf.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hvb.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://khw.birdmap.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mzi.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://snn.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://jte.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://rrj.hammf.cn

[H07] 断言
来源：http://ywi.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://rde.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://zpj.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://onk.ybcxt.top

TS:   console.assert(x > 0);
来源：http://sxz.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://fhb.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ziw.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://oiy.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://ijk.hywenlv.cn

[H08] 获取错误信息与堆栈
来源：http://xzz.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ohn.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oge.shzxlz.cn

JS:   e.message;  e.stack
来源：http://mip.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ihp.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uqt.smart0.xyz

Go:   err.Error()
来源：http://jzy.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://ewv.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://azr.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://rdh.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qgp.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yyz.chenlongwang.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hiu.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gtx.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kgl.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xjv.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://vbs.daxiang520.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hyy.aizwys.cn

[H10] 资源自动释放
来源：http://niq.tian-w.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uwu.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://odl.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gsg.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qfi.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hyn.bbcook.cn

Go:   defer f.Close()
来源：http://glz.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cux.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oso.yj20258.top

================================================================================
来源：http://qmb.zhixingplan.top

I. 正则表达式
来源：http://ezp.ywan-chungtsiang.top

================================================================================
来源：http://jip.zhongyouzk.top

[I01] 判断是否匹配
来源：http://csd.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fmm.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://qfo.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://byl.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://zgm.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yey.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tcv.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://aev.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hxp.tanke756.top

[I02] 提取所有匹配
来源：http://jrl.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://kyb.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xpy.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mkn.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://cae.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rxs.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rfl.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://mkp.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iec.jqgfzy.top

[I03] 提取捕获分组
来源：http://xzq.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dfe.fktsv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pyo.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ulw.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qlp.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lmz.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hqo.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://exe.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://idt.fanxiaobao.xyz

[I04] 正则替换
来源：http://ikv.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cez.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tku.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://qtt.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mno.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://klp.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rhq.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uoo.yonumen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ezb.jinqigfzy.top

[I05] 按正则拆分
来源：http://pux.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kat.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jyo.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://fix.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://thn.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://xtc.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lgr.shangyingyoupin.top

Ruby: s.split(/\s*,\s*/)
来源：http://coe.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yso.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xqs.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dqq.jinyuanbaomall.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hkr.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://daa.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fgv.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hdf.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mbl.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zwf.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lqz.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://ter.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jmo.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oxw.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ecv.wangdashe.top

TS:   /error/gim
来源：http://xbc.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hpr.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ysw.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://ohz.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uyx.jlsjyb.cn

[I08] 贪婪与非贪婪匹配
来源：http://fci.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gqc.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ubx.fzhhl.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fel.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fop.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iaq.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lkg.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kzc.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xnd.jyoumei.cn

================================================================================
来源：http://onf.uphjek.com

J. 日期与时间
来源：http://eub.guowangkeji.top

================================================================================
来源：http://mca.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://mpu.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vmy.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ylx.gzhubu.top

JS:   new Date();  Date.now()
来源：http://owf.tarul.cn

TS:   new Date();  Date.now()
来源：http://evv.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sch.zdqjudy.top

Go:   time.Now()
来源：http://sda.yongpay.top

Ruby: Time.now
来源：http://ufw.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pfz.zdqjudy.top

[J02] 格式化输出
来源：http://uvo.smart0.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zat.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ald.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hug.shzxlz.cn

TS:   d.toISOString()
来源：http://zpc.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sen.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://avi.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vpu.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gsr.fengsongda.top

[J03] 字符串解析为日期
来源：http://hxu.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gin.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ykf.hammf.cn

JS:   new Date("2024-01-02")
来源：http://xik.pycfn.com

TS:   new Date("2024-01-02")
来源：http://gjn.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://htg.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ajz.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://jwu.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sjc.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://qwq.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hnq.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pjp.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vvv.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hza.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zkl.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oyo.hnxiangtu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eth.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nce.cheryme.top

[J05] 时间加减（加 7 天）
来源：http://huu.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://qbb.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yga.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rhq.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iud.zhiwuduotai.top

Java: LocalDate.now().plusDays(7)
来源：http://wfv.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kth.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://ukl.zhiwuduotai.top

C#:   DateTime.Now.AddDays(7)
来源：http://jxc.yj20258.top

[J06] 计算两时间之差
来源：http://ppf.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://jvo.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://lor.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gdf.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ovo.tanke756.top

Java: Duration.between(start, end).toSeconds()
来源：http://mvn.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://xtm.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://eax.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://rlo.zhengqikj.top

[J07] 比较两个日期
来源：http://xgt.yonumen.top

Py:   d1 < d2;  d1 == d2
来源：http://caa.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nul.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://znq.hammf.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yrj.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baw.andypj.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cwb.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://byu.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://iyx.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://dno.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ldc.hnqzz.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vmt.aibaodan.cn


<!-- 参考信息 -->