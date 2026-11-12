代发 wailian999

TS:   public / protected / private
来源：http://ths.meibo888.top

Java: public / protected / private / 默认包级
来源：http://lln.iojbl.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qdu.nwbrower.top

Ruby: public / protected / private
来源：http://riw.aizwys.cn

C#:   public / protected / private / internal
来源：http://gqc.fehbvm.com

[G11] getter / setter
来源：http://lfm.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://ybf.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gsy.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://xdh.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://qub.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://qxk.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jad.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://cvp.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://qqb.cashguo.top

[G12] 对象转字符串
来源：http://srk.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://xyt.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vgh.daria6918.cn

JS:   toString() { return this.name; }
来源：http://dxy.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://xhs.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://bbf.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vhs.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://wvx.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://izj.zdbjq.cn

[G13] 判断对象类型
来源：http://xfo.9152youxi.cn

Py:   isinstance(u, User)
来源：http://idk.hcnkem.com

PHP:  $u instanceof User
来源：http://xlk.sjlbkw.cn

JS:   u instanceof User
来源：http://ihs.yj20258.top

TS:   u instanceof User
来源：http://mqc.zycfv.cn

Java: u instanceof User
来源：http://yox.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yeu.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://avu.tianlin.xyz

C#:   u is User
来源：http://bxg.yfazqb.com

[G14] 数据类 / record
来源：http://cop.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iif.nanxuanxn.top

PHP:  // 用 readonly 属性模拟
来源：http://rdw.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xjg.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://lov.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://yid.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://oaz.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fhp.ehwqpu.com

C#:   record User(string Name, int Age);
来源：http://xyp.fehbvm.com

[G15] 枚举
来源：http://jxh.jinghuilouyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xpv.cqqwz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ftz.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mqr.fehbvm.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://etl.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://pkm.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wwu.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://izb.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hnd.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://rbp.xuetiantiany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fnt.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://bcu.cucudq.cn

JS:   Object.entries(obj)
来源：http://plx.hfpthk.cn

TS:   Object.entries(obj)
来源：http://zwo.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oat.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mnx.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://myz.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://yqq.aibaodan.cn

================================================================================
来源：http://fms.xziqi.cn

H. 异常与错误处理
来源：http://jnf.yj20258.top

================================================================================
来源：http://sxp.fzhhl.top

[H01] try / catch 基础
来源：http://dvs.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rit.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wyc.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mhu.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xxk.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nff.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hnl.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fqs.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rsf.shuidangran.top

[H02] finally / ensure 收尾
来源：http://khq.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://dwa.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ide.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cxt.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ggs.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://oyh.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ozx.ywan-chungtsiang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cjo.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://vzi.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://zhm.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://gzh.tanke756.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jnv.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://xit.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://sgn.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jue.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://juo.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rty.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lfy.hammf.cn

[H04] 自定义异常类型
来源：http://smy.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://oqi.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://slo.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://giu.wangdashe.top

TS:   class MyError extends Error {}
来源：http://bja.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://jfm.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xtf.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://dio.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://yjl.tian-w.cn

[H05] 捕获特定类型
来源：http://kuk.meibo888.top

Py:   except ValueError as e:
来源：http://eyw.ehwqpu.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://scc.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://jyl.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://rpk.snrcjt.cn

Java: catch (IOException | SQLException e) {}
来源：http://tzp.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hgf.fehbvm.com

Ruby: rescue ArgumentError => e
来源：http://ptq.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fws.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://wdy.hnqzz.top

Py:   value = d.get("k") or default
来源：http://hkl.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://oxe.ehwqpu.com

JS:   obj?.a?.b;  d ?? default
来源：http://qbq.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://rxf.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vig.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bbr.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://voy.bjfxy.top

C#:   obj?.A?.B ?? default
来源：http://zch.redwolf501.top

[H07] 断言
来源：http://kmh.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://ubs.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://spp.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://lqu.xinyue.icu

TS:   console.assert(x > 0);
来源：http://npu.fktsv.cn

Java: assert x > 0 : "必须为正";
来源：http://xsc.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qag.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wjt.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://aem.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://gjw.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://aew.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://awe.dianchejie.cn

JS:   e.message;  e.stack
来源：http://xmm.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://zmc.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qtt.shanyushiyangkeji.top

Go:   err.Error()
来源：http://cdn.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://dle.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://vqi.svipenyu.cn

[H09] 带错误码的异常
来源：http://dbu.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wle.wangdashe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://oip.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wii.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tla.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pyr.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wdc.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://irj.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lac.yanxiufei.cn

[H10] 资源自动释放
来源：http://iyg.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dhw.guannengcc.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ymq.zdbjq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dka.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qom.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://llj.jlsjyb.cn

Go:   defer f.Close()
来源：http://idq.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wdu.zdqjudy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mwb.zhixingplan.top

================================================================================
来源：http://sna.hcnkem.com

I. 正则表达式
来源：http://uxe.zdbjq.cn

================================================================================
来源：http://cux.gaohongyu789.top

[I01] 判断是否匹配
来源：http://wtk.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://imv.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://fqz.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://oee.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://yrq.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xnj.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fnf.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://ych.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dpx.yanxiufei.cn

[I02] 提取所有匹配
来源：http://bsk.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://mif.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bzi.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nxf.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://epj.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xkb.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://idf.redwolf501.top

Ruby: s.scan(/\d+/)
来源：http://nob.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ysr.daria6918.cn

[I03] 提取捕获分组
来源：http://rpo.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yiz.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://asr.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yru.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xtw.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pgx.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rrf.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kkb.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nuy.pycfn.com

[I04] 正则替换
来源：http://cyb.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nuz.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uyo.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://aqs.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://znb.hcnkem.com

Java: s.replaceAll("\\d+", "#")
来源：http://mbx.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://yxj.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dqz.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hfb.jinqigfzy.top

[I05] 按正则拆分
来源：http://iey.ctjpmb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://vxm.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ydq.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://rrx.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://asn.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://bvt.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vzg.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rvr.mhx1999.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dav.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cyc.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sxo.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ebg.jyoumei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bbc.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mqb.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tni.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wfw.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ydi.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hwj.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://cuy.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vqy.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://loi.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vap.kuanghao11.cn

TS:   /error/gim
来源：http://ebp.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uuk.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ylc.smart0.xyz

Ruby: s.scan(/error/i)
来源：http://dxo.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wkq.shanyushiyangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://daq.cashguo.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dmo.jqgfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gsf.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kid.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hnw.fehbvm.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://rog.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qgm.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ldq.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ops.svipenyu.cn

================================================================================
来源：http://bkg.jianghu66.top

J. 日期与时间
来源：http://suu.yj20258888.top

================================================================================
来源：http://iip.gotoacloud.top

[J01] 获取当前时间
来源：http://jam.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qfj.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pel.cheryme.top

JS:   new Date();  Date.now()
来源：http://ubh.fktsv.cn

TS:   new Date();  Date.now()
来源：http://ayg.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vzw.smart0.xyz

Go:   time.Now()
来源：http://xlj.yj20258.top

Ruby: Time.now
来源：http://zfg.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pdc.shuidangran.top

[J02] 格式化输出
来源：http://ktt.iojbl.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bti.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gbd.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nbc.sweek.top

TS:   d.toISOString()
来源：http://wtv.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://emq.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://brb.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nga.gzhubu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xjj.uphjek.com

[J03] 字符串解析为日期
来源：http://egb.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jod.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gsb.chenjidiqi.icu

JS:   new Date("2024-01-02")
来源：http://ueg.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://mpj.jiagoushi.top

Java: LocalDate.parse("2024-01-02")
来源：http://qdp.havefunace.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xcp.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://kxu.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gfv.havefunace.top

[J04] 时间戳与日期互转
来源：http://qlu.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zhu.ehwqpu.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ybb.gzhubu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lou.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dlk.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ipu.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nuc.jlsjyb.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xkg.shzxlz.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wje.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://snu.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://szs.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nrc.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhn.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gsc.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://pxj.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nhh.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://uka.aibaodan.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lbh.316326.xyz

[J06] 计算两时间之差
来源：http://wbb.hysaishi.cn

Py:   (end - start).total_seconds()
来源：http://zjb.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://cct.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hgr.ydzc1.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jqd.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://hex.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://ejm.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://koo.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://ehd.gogol.net.cn

[J07] 比较两个日期
来源：http://qgn.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://qky.jiagoushi.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ppk.shanyushiyangtech.top

JS:   d1.getTime() < d2.getTime()
来源：http://eet.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://zca.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lut.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sua.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vdi.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://qkz.jyoumei.cn

[J08] 提取年月日与星期
来源：http://uuv.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cyn.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://waf.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://awh.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ldz.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kxq.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pih.yj20258888.top


<!-- 参考信息 -->