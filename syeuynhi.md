代发 wailian999

[G10] 访问控制
来源：http://zbw.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://rec.yanxiufei.cn

PHP:  public / protected / private
来源：http://mcy.fengsongda.top

JS:   #private 字段；其余公开
来源：http://xvz.zhongyouzk.top

TS:   public / protected / private
来源：http://wnw.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://nbu.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jlh.hcnkem.com

Ruby: public / protected / private
来源：http://typ.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://ccm.ydzc1.top

[G11] getter / setter
来源：http://ihq.daria6918.cn

Py:   @property 与 @x.setter
来源：http://xdl.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://fsn.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://aks.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://cln.mhx1999.top

Java: public String getName() { return name; }
来源：http://thj.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://drl.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://rdo.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://all.ppjwa.cn

[G12] 对象转字符串
来源：http://vrv.birdmap.top

Py:   def __str__(self): return self.name
来源：http://sgh.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://egn.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://etz.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://xuo.sweek.top

Java: @Override public String toString() { return name; }
来源：http://aqh.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rdv.epnwcf.com

Ruby: def to_s; @name; end
来源：http://rfk.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://ngv.nwbrower.top

[G13] 判断对象类型
来源：http://xii.zdbjq.cn

Py:   isinstance(u, User)
来源：http://bqt.chenlongwang.top

PHP:  $u instanceof User
来源：http://tox.andypj.xyz

JS:   u instanceof User
来源：http://dod.shanyushiyangtech.top

TS:   u instanceof User
来源：http://zii.hcnkem.com

Java: u instanceof User
来源：http://mjk.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://zwf.316326.xyz

Ruby: u.is_a?(User)
来源：http://hkk.jyoumei.cn

C#:   u is User
来源：http://oaf.xziqi.cn

[G14] 数据类 / record
来源：http://uhk.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://upz.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://zwg.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://keo.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://czr.yj20258.top

Java: record User(String name, int age) {}
来源：http://voz.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://xlj.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://beg.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://bea.guowangkeji.top

[G15] 枚举
来源：http://pxz.guowangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://euj.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jud.zhoulong.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://znj.ydjk.org.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://obx.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://aos.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rbu.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://ayw.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hlf.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://gxq.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://myx.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://zjp.xinyue.icu

JS:   Object.entries(obj)
来源：http://okx.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://myu.epnwcf.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ocg.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tsk.shzxlz.cn

Ruby: obj.instance_variables
来源：http://kcq.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://bzo.c1oappe.top

================================================================================
来源：http://bar.gzhubu.top

H. 异常与错误处理
来源：http://qln.sysykeji.top

================================================================================
来源：http://efb.wangshuangyany.cn

[H01] try / catch 基础
来源：http://siz.cashguo.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://afs.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://whx.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wfa.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jhf.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wlg.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ily.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://riu.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uum.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://wtg.shanyushiyangtech.top

Py:   try: f()⏎finally: cleanup()
来源：http://ehm.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://qcn.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gxc.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://clh.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pfq.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qwk.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uhp.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uua.tarul.cn

[H03] 主动抛出异常
来源：http://dfi.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://ryj.ywan-chungtsiang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jum.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://vps.cashguo.top

TS:   throw new Error("错误信息");
来源：http://wlf.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://owo.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ide.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://jcf.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kmu.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://zuz.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://gds.yj20258888.top

PHP:  class MyError extends RuntimeException {}
来源：http://qtp.uphjek.com

JS:   class MyError extends Error {}
来源：http://lth.xylfe.cn

TS:   class MyError extends Error {}
来源：http://rlx.zhoulong.xyz

Java: class MyException extends RuntimeException {}
来源：http://dgo.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hgn.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://xom.smart0.xyz

C#:   class MyException : Exception {}
来源：http://ujh.kuanghao11.cn

[H05] 捕获特定类型
来源：http://kve.sufxvd.cn

Py:   except ValueError as e:
来源：http://lnh.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sim.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://gqe.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://bcx.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://ipe.gotoacloud.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sro.wangshuangyany.cn

Ruby: rescue ArgumentError => e
来源：http://lpa.pycfn.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kcj.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://uxw.yj20258888.top

Py:   value = d.get("k") or default
来源：http://yuv.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ysa.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://liv.gotoacloud.top

TS:   obj?.a?.b;  d ?? default
来源：http://fmz.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uzu.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zwx.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://avh.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://ohw.xingfuxueyuan.xyz

[H07] 断言
来源：http://xvu.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://jpe.ppjwa.cn

PHP:  assert($x > 0);
来源：http://eut.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://xfk.cashguo.top

TS:   console.assert(x > 0);
来源：http://qql.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://ooi.sjlbkw.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://psn.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xtn.jiagoushi.top

C#:   Debug.Assert(x > 0);
来源：http://xit.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://xnp.sjlbkw.cn

Py:   str(e);  traceback.format_exc()
来源：http://rof.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oxd.wangdashe.top

JS:   e.message;  e.stack
来源：http://jiv.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://vyw.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://isr.cucudq.cn

Go:   err.Error()
来源：http://fbz.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://xum.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://xqu.gzhubu.top

[H09] 带错误码的异常
来源：http://blq.sxryk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nhd.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tvq.snrcjt.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://txl.tianlin.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://epb.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://amm.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fph.ehwqpu.com

Ruby: raise MyError.new("fail", 500)
来源：http://akf.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vyf.nanxinkj.top

[H10] 资源自动释放
来源：http://trv.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ssp.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wkl.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://znc.xuanzx.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yan.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jcu.nanxinkj.top

Go:   defer f.Close()
来源：http://hvq.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mgw.epnwcf.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bdu.316326.xyz

================================================================================
来源：http://fom.0kj1m.cn

I. 正则表达式
来源：http://sdd.cashguo.top

================================================================================
来源：http://lfx.dashuyun.cn

[I01] 判断是否匹配
来源：http://qbz.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tsu.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://gso.cashguo.top

JS:   /\d+/.test(s)
来源：http://fhw.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://kim.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uau.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mul.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://kjg.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sru.zhongyouzk.top

[I02] 提取所有匹配
来源：http://xnq.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://iae.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ays.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://agx.shzxlz.cn

TS:   s.match(/\d+/g)
来源：http://lrk.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wgu.yj20258.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kzs.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://ruy.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tdu.ppjwa.cn

[I03] 提取捕获分组
来源：http://sth.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cnl.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://prd.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vwh.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://drt.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jmp.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hoj.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zzo.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qzd.shuidangran.top

[I04] 正则替换
来源：http://gpg.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yje.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hvj.yuanzhike.top

JS:   s.replace(/\d+/g, "#")
来源：http://zmj.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://kug.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://gcw.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qne.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lxk.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iyu.fehbvm.com

[I05] 按正则拆分
来源：http://lcr.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://aan.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://api.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://gwu.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://zwl.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://ryp.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mhp.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jeq.cashguo.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ijr.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tbn.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kxa.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wac.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pxy.jiagoushi.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kbt.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tdw.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://thq.snrcjt.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uul.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kvk.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://eau.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lep.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hyr.zycfv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yxe.c1oappe.top

TS:   /error/gim
来源：http://lqp.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ibl.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yqo.yonumen.top

Ruby: s.scan(/error/i)
来源：http://fgm.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ycm.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://bdk.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eir.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://orb.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dxf.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://awx.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cvt.quarkkingdee.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vmr.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dfo.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qgy.0kj1m.cn

================================================================================
来源：http://emm.gogol.net.cn

J. 日期与时间
来源：http://eki.tian-w.cn

================================================================================
来源：http://cpw.tian-w.cn

[J01] 获取当前时间
来源：http://gqs.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wvg.xuanzx.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uxr.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://fya.jqgfzy.top

TS:   new Date();  Date.now()
来源：http://oyi.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://sph.chenlongwang.top

Go:   time.Now()
来源：http://bpe.xuetiantiany.cn

Ruby: Time.now
来源：http://vxc.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wxl.ppjwa.cn

[J02] 格式化输出
来源：http://dym.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://irs.vehdjk.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wey.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vqm.ydzc1.top

TS:   d.toISOString()
来源：http://upg.zhiwuduotai.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fno.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hwm.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kxz.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://asu.yongpay.top

[J03] 字符串解析为日期
来源：http://xfp.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://njm.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ozg.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://wuq.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://qbw.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vev.xziqi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pkj.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://cdh.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fay.hesvh.cn

[J04] 时间戳与日期互转
来源：http://ebm.ydjk.org.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tcy.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bso.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kek.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vkn.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ste.haohaochexian.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sxo.tanke756.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://crn.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xpm.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://rig.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://tmo.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://upg.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbg.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uvd.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://shd.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dpd.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://ooc.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://iss.zycfv.cn

[J06] 计算两时间之差
来源：http://uqk.cdnleiting.top

Py:   (end - start).total_seconds()
来源：http://cvx.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://hqa.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xiz.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://api.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://icu.gaohongyu789.top

Go:   end.Sub(start).Hours()
来源：http://eip.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://she.hywenlv.cn

C#:   (end - start).TotalSeconds
来源：http://dgb.0kj1m.cn

[J07] 比较两个日期
来源：http://vix.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://kgr.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ljr.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://xts.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://dvu.pengpengdd.cyou

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ksm.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mrw.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://gok.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://lcv.haohaochexian.top

[J08] 提取年月日与星期
来源：http://zly.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dii.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://huk.hesvh.cn


<!-- 参考信息 -->