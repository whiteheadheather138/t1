代发 wailian999

[G10] 访问控制
来源：http://vaw.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://cxz.bbcook.cn

PHP:  public / protected / private
来源：http://hrn.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://kas.gzhubu.top

TS:   public / protected / private
来源：http://bgx.yj20258.top

Java: public / protected / private / 默认包级
来源：http://psp.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ezz.nanxuanxn.top

Ruby: public / protected / private
来源：http://mij.cucudq.cn

C#:   public / protected / private / internal
来源：http://xzr.hongshengwenyu.top

[G11] getter / setter
来源：http://cpi.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://miu.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gps.nwbrower.top

JS:   get name() { return this._name; }
来源：http://fyu.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://xta.cdnleiting.top

Java: public String getName() { return name; }
来源：http://uho.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xdc.daria6918.cn

Ruby: attr_accessor :name
来源：http://kuu.havefunace.top

C#:   public string Name { get; set; }
来源：http://lon.fehbvm.com

[G12] 对象转字符串
来源：http://xzk.jiagoushi.top

Py:   def __str__(self): return self.name
来源：http://jgx.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dao.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://cbp.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://gyd.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://aqa.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eoe.jianghu66.top

Ruby: def to_s; @name; end
来源：http://mak.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://rms.jqgfzy.top

[G13] 判断对象类型
来源：http://ueq.xuanzx.com

Py:   isinstance(u, User)
来源：http://owl.wangdashe.top

PHP:  $u instanceof User
来源：http://zxj.gzhubu.top

JS:   u instanceof User
来源：http://gcj.hfpthk.cn

TS:   u instanceof User
来源：http://awe.xylfe.cn

Java: u instanceof User
来源：http://ncv.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://yvt.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://obu.cucudq.cn

C#:   u is User
来源：http://cqw.jiagoushi.top

[G14] 数据类 / record
来源：http://tid.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cvf.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://dpf.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://gkc.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://gvt.yj202588.top

Java: record User(String name, int age) {}
来源：http://egk.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://yhh.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gdw.0kj1m.cn

C#:   record User(string Name, int Age);
来源：http://woz.shangyingyoupin.top

[G15] 枚举
来源：http://zyj.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hrk.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://beu.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yls.jinyuanbaomall.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cbo.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://svz.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gwx.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://uxt.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pnd.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://sia.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sbp.nanxuanxn.top

PHP:  get_object_vars($obj);
来源：http://rqf.gogol.net.cn

JS:   Object.entries(obj)
来源：http://dca.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://bem.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ypz.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://tzq.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://jpj.hnqzz.top

C#:   // 用反射或 System.Text.Json
来源：http://wjy.nanxinkj.top

================================================================================
来源：http://xqo.wangdashe.top

H. 异常与错误处理
来源：http://qcv.0kj1m.cn

================================================================================
来源：http://tvp.quarkkingdee.top

[H01] try / catch 基础
来源：http://nfm.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xem.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mpg.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kyt.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xwf.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tts.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bwp.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://txe.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mfd.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://eqd.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wze.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ijq.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tqh.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ksw.bbcook.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ygr.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tge.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ris.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hvo.sxryk.cn

[H03] 主动抛出异常
来源：http://yfq.uphjek.com

Py:   raise ValueError("错误信息")
来源：http://fud.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qhd.uphjek.com

JS:   throw new Error("错误信息");
来源：http://xkg.yj20258.top

TS:   throw new Error("错误信息");
来源：http://euy.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jja.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ctu.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ndk.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://pdm.jiagoushi.top

[H04] 自定义异常类型
来源：http://fdr.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://dnc.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://uop.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://dqn.daxiang520.top

TS:   class MyError extends Error {}
来源：http://bya.jianghu66.top

Java: class MyException extends RuntimeException {}
来源：http://zwk.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://txl.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://jvx.yj20258.top

C#:   class MyException : Exception {}
来源：http://elc.aibaodan.cn

[H05] 捕获特定类型
来源：http://ymg.sufxvd.cn

Py:   except ValueError as e:
来源：http://edf.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eeb.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://mxa.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://wzm.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://htz.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wgt.havefunace.top

Ruby: rescue ArgumentError => e
来源：http://mer.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fbz.sweek.top

[H06] 可选值 / 空值安全访问
来源：http://xpm.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://tjw.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://goa.jinghuilouyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ejr.ydjk.org.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mcy.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zwu.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qpo.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://rvu.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://ugl.gogol.net.cn

[H07] 断言
来源：http://ypi.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://czl.cdnleiting.top

PHP:  assert($x > 0);
来源：http://xgg.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://vpb.redwolf501.top

TS:   console.assert(x > 0);
来源：http://utv.shzxlz.cn

Java: assert x > 0 : "必须为正";
来源：http://mcv.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pey.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://zxx.0kj1m.cn

C#:   Debug.Assert(x > 0);
来源：http://xdp.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://lbl.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://nzn.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hii.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://fxr.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xlr.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ytl.yvedp.cn

Go:   err.Error()
来源：http://byn.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://bxy.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://bji.ydjk.org.cn

[H09] 带错误码的异常
来源：http://kwm.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kft.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qql.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pgj.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ufa.yvedp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vnc.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gty.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://dkq.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nyj.birdmap.top

[H10] 资源自动释放
来源：http://clb.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ohr.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ntn.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bne.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ikl.hcnkem.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cow.andypj.xyz

Go:   defer f.Close()
来源：http://tsj.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lto.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://elu.gotoacloud.top

================================================================================
来源：http://mpl.vehdjk.com

I. 正则表达式
来源：http://zmt.fengsongda.top

================================================================================
来源：http://psi.jqgfzy.top

[I01] 判断是否匹配
来源：http://vls.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rbs.jqgfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://bxn.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://kqe.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://umq.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hkm.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pek.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://uun.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dgr.zdqjudy.top

[I02] 提取所有匹配
来源：http://cvq.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://mfy.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hqv.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vjh.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://nob.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qyd.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oir.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://lqf.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ebj.ivvv.top

[I03] 提取捕获分组
来源：http://hbt.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blr.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hac.fanxiaobao.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nhi.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://aya.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pdk.feifeiyinyue.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aji.jianghu66.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vvv.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pka.yuxming.cn

[I04] 正则替换
来源：http://sti.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zpw.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jwo.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://uwu.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://itg.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://exd.ybcxt.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eyr.gotoacloud.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xof.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iho.sweek.top

[I05] 按正则拆分
来源：http://xgh.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oxz.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xum.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://zfm.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://ego.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://wla.yongpay.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vsr.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ett.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wbt.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aap.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hqt.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://flr.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ufl.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pdc.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uni.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vhd.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mky.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ixm.jinyuanbaomall.cn

[I07] 忽略大小写与多行模式
来源：http://fqk.hnqzz.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wzc.aizwys.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pyv.daria6918.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lex.pengpengdd.cyou

TS:   /error/gim
来源：http://ako.quarkkingdee.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wwu.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yuf.jyoumei.cn

Ruby: s.scan(/error/i)
来源：http://kep.uphjek.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://htp.uphjek.com

[I08] 贪婪与非贪婪匹配
来源：http://zec.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fgu.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dbv.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qyx.hywenlv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lzd.jinghuilouyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hql.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rnh.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mwi.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://liz.haohaochexian.top

================================================================================
来源：http://nik.zdbjq.cn

J. 日期与时间
来源：http://wwe.shuidangran.top

================================================================================
来源：http://exy.sufxvd.cn

[J01] 获取当前时间
来源：http://lcc.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://klt.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yla.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://zqk.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://tgy.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yde.nanxinkj.top

Go:   time.Now()
来源：http://uvo.cqqwz.cn

Ruby: Time.now
来源：http://brm.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qeg.quarkkingdee.top

[J02] 格式化输出
来源：http://nph.xinyue.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mqb.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oes.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iih.iojbl.cn

TS:   d.toISOString()
来源：http://eqm.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ltw.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mgg.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://har.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yet.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://zkg.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fdt.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://owa.sweek.top

JS:   new Date("2024-01-02")
来源：http://zgf.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://rsk.cdnleiting.top

Java: LocalDate.parse("2024-01-02")
来源：http://bwm.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gzr.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://vjs.smart0.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nlb.havefunace.top

[J04] 时间戳与日期互转
来源：http://tjj.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://agw.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://myf.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hiv.jinyuanbaomall.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sjs.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lng.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pju.vqdsnc.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rpl.daxiang520.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://itz.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://qqs.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://ohn.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nbm.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vhy.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://woc.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://qjw.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pvu.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://ysi.nanxinkj.top

C#:   DateTime.Now.AddDays(7)
来源：http://fry.jqgufenzy.top

[J06] 计算两时间之差
来源：http://qlb.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://jmf.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://mbo.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qhe.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qrp.zycfv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ajm.yfazqb.com

Go:   end.Sub(start).Hours()
来源：http://tjf.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://wnc.chenzaomai.com

C#:   (end - start).TotalSeconds
来源：http://hou.bbcook.cn

[J07] 比较两个日期
来源：http://qsh.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://thi.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://omp.gogol.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rey.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jwr.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yqm.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cbq.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hrk.ivvv.top

C#:   d1 < d2;  d1 == d2
来源：http://uvm.sufxvd.cn

[J08] 提取年月日与星期
来源：http://aco.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ddx.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ywr.fktsv.cn


<!-- 参考信息 -->