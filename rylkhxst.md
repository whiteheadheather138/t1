代发 wailian999

[Q65] 回滚事务
来源：http://icv.shuidangran.top

ROLLBACK;
来源：http://npo.0kj1m.cn

[Q66] 行锁查询
来源：http://eun.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ooe.yfazqb.com

[Q67] 设置隔离级别
来源：http://zps.jinyuanbaomall.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vbh.shuidangran.top

[Q68] 保存点
来源：http://faz.chenjidiqi.icu

SAVEPOINT sp1;
来源：http://jdu.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://six.wangshuangyany.cn

[Q69] 查看执行计划
来源：http://pyj.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xpy.316326.xyz

[Q70] 更新统计信息
来源：http://lpp.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://mlv.guannengcc.top

[Q71] 查看建表语句
来源：http://bta.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ozu.jlsjyb.cn

[Q72] 查看索引
来源：http://krm.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://qnk.gogol.net.cn

[Q73] 查看表状态
来源：http://ovq.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wev.bjfxy.top

[Q74] 强制使用索引
来源：http://oyv.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bvl.guannengcc.top

[Q75] 日期格式化
来源：http://rsw.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fpq.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nse.hysaishi.cn

[Q76] 按天统计
来源：http://tdf.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mhq.uphjek.com

[Q77] 时间加减
来源：http://wyj.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://umj.yanxiufei.cn

[Q78] 当前时间
来源：http://qcn.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kqj.chenzaomai.com

[Q79] 字符串拼接
来源：http://lac.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bzw.zhixingplan.top

[Q80] 字符串截取
来源：http://upi.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kor.bjfxy.top

[Q81] 字符串替换
来源：http://zfv.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fub.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://jde.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jdp.gogol.net.cn

[Q83] 大小写转换
来源：http://zli.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kdn.chenzaomai.com

[Q84] 去除首尾空格
来源：http://gyf.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://bvb.sysykeji.top

[Q85] 数值取整
来源：http://xwc.shzxlz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qct.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://aum.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lfz.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://oem.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gtu.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://cdm.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://saz.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fft.zhengqikj.top

[Q89] 判断表是否存在
来源：http://rsf.zhengqikj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tkq.vehdjk.com

[Q90] 生成序号列
来源：http://fsv.hnxiangtu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qhd.vqdsnc.cn

================================================================================
来源：http://hci.chenzaomai.com

R. Bash 专题
来源：http://may.feifeiyinyue.top

================================================================================
来源：http://obd.ybcxt.top

[R01] shebang 与严格模式
来源：http://dfn.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://brd.yongpay.top

set -euo pipefail
来源：http://lve.zhengqikj.top

[R02] 变量赋值与使用
来源：http://ulu.zdbjq.cn

name="Tom"; echo "$name"
来源：http://nwq.gotoacloud.top

[R03] 只读变量
来源：http://kur.fzhhl.top

readonly PI=3.14
来源：http://sxw.tianlin.xyz

[R04] 位置参数
来源：http://cga.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jsf.vehdjk.com

[R05] 参数默认值
来源：http://gnu.316326.xyz

name="${1:-default}"
来源：http://qnb.kuanghao11.cn

[R06] 判断命令是否存在
来源：http://gpq.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xww.fktsv.cn

[R07] if 判断文件
来源：http://nur.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lit.aibaodan.cn

[R08] 数值比较
来源：http://aah.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wwy.yuxming.cn

[R09] 字符串比较
来源：http://aui.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cyt.yueranfly.top

[R10] 正则匹配
来源：http://rco.hnqzz.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dky.redwolf501.top

[R11] case 多分支
来源：http://pgf.hnqzz.top

case "$1" in
来源：http://rht.svipenyu.cn

start) echo "启动" ;;
来源：http://wqb.fktsv.cn

stop)  echo "停止" ;;
来源：http://rza.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://btu.yuanzhike.top

esac
来源：http://gip.zhongyouzk.top

[R12] for 遍历文件
来源：http://iba.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://qsn.zycfv.cn

[R13] for 计数循环
来源：http://eyl.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://xkv.nanxinkj.top

[R14] C 风格 for
来源：http://dbe.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tbq.xinyue.icu

[R15] while 逐行读文件
来源：http://cdf.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://htt.jinyuanbaomall.cn

[R16] until 等待条件
来源：http://ryc.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bqx.pengpengdd.cyou

[R17] 数组定义与取值
来源：http://koe.zhongyouzk.top

arr=(a b c); echo "${arr[0]}"
来源：http://zhu.cqqwz.cn

[R18] 遍历数组
来源：http://gys.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pnk.havefunace.top

[R19] 数组长度
来源：http://mdf.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://uod.daxiang520.top

[R20] 关联数组（字典）
来源：http://vyq.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://onp.vehdjk.com

[R21] 字符串长度
来源：http://che.redwolf501.top

echo "${#s}"
来源：http://lvg.fanxiaobao.xyz

[R22] 截取子串
来源：http://vtx.haohaochexian.top

echo "${s:0:5}"
来源：http://rsm.sysykeji.top

[R23] 字符串替换
来源：http://zbr.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bqx.xylfe.cn

[R24] 大小写转换
来源：http://nzh.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://hej.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://oqg.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pso.sjlbkw.cn

[R26] 命令替换
来源：http://pdd.pycfn.com

now=$(date +%F); echo "$now"
来源：http://kwv.ydzc1.top

[R27] 算术展开
来源：http://wau.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://oif.uphjek.com

[R28] 浮点运算
来源：http://jvv.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://fxz.svipenyu.cn

[R29] 定义函数
来源：http://kat.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pfv.ydjk.org.cn

[R30] 函数返回状态码
来源：http://pas.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://cry.shuidangran.top

[R31] 局部变量
来源：http://qlv.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://gva.sxryk.cn

[R32] 参数个数校验
来源：http://deh.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sws.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://vwx.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://puv.kuanghao11.cn

[R34] 退出时清理
来源：http://imp.yonumen.top

trap 'rm -f "$tmp"' EXIT
来源：http://sah.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://bhn.zdqjudy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://exs.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://hjd.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rfo.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://qwb.quarkkingdee.top

files=$(ls -1)
来源：http://hbs.pycfn.com

[R38] 管道串联
来源：http://hkz.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://ybz.316326.xyz

[R39] 重定向标准输出与错误
来源：http://gnr.jyoumei.cn

cmd > out.log 2>&1
来源：http://exj.quarkkingdee.top

[R40] 追加写日志
来源：http://lec.0kj1m.cn

echo "log" >> out.log
来源：http://pol.vqdsnc.cn

[R41] 丢弃输出
来源：http://uwz.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://xpp.chenzaomai.com

[R42] 输入重定向
来源：http://qxw.gaohongyu789.top

wc -l < a.txt
来源：http://mng.gzhubu.top

[R43] 按名字查找文件
来源：http://jqw.aizwys.cn

find . -name "*.log" -type f
来源：http://yxj.guannengcc.top

[R44] 按修改时间查找
来源：http://hkl.xziqi.cn

find . -mtime -7 -type f
来源：http://zix.jqgfzy.top

[R45] 批量删除
来源：http://ood.nwbrower.top

find . -name "*.tmp" -delete
来源：http://uqo.havefunace.top

[R46] 递归替换文件内容
来源：http://hnf.hfpthk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tda.zdqjudy.top

[R47] sed 单行替换
来源：http://qhb.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://hic.sufxvd.cn

[R48] awk 取指定列
来源：http://pde.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://omd.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://ntn.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vyz.yvedp.cn

[R50] awk 求和
来源：http://nlc.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://dyn.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://dpn.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://isr.ehwqpu.com

[R52] 统计行数
来源：http://man.xingfuxueyuan.xyz

wc -l a.txt
来源：http://woq.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://cpu.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://biq.hysaishi.cn

[R54] 比较两个文件
来源：http://fuu.sweek.top

diff a.txt b.txt
来源：http://qqb.hammf.cn

[R55] 压缩与解压
来源：http://nrf.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jlc.hysaishi.cn

[R56] 远程拷贝
来源：http://cdx.jyoumei.cn

scp file user@host:/path/
来源：http://cdn.birdmap.top

[R57] 远程执行命令
来源：http://rmp.quarkkingdee.top

ssh user@host 'uptime'
来源：http://peo.dashuyun.cn

[R58] 下载文件
来源：http://ucf.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nel.guannengcc.top

[R59] 发 POST JSON
来源：http://miy.shanyushiyangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://akq.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://ats.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yvs.andypj.xyz

[R61] 磁盘占用
来源：http://ssb.jyoumei.cn

df -h;  du -sh *
来源：http://ieb.yuxming.cn

[R62] 找最占空间的文件
来源：http://jym.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://qke.jinghuilouyu.cn

[R63] 内存与进程
来源：http://hlw.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://afe.hnqzz.top

[R64] 结束进程
来源：http://bnb.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://fmz.wangshuangyany.cn

[R65] 查看端口占用
来源：http://old.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xgb.gogol.net.cn

[R66] 定时任务
来源：http://aqk.iojbl.cn

crontab -e;  crontab -l
来源：http://muj.bjfxy.top

[R67] 生成随机十六进制串
来源：http://suv.sjlbkw.cn

openssl rand -hex 16
来源：http://fff.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://kwd.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://bfw.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://ist.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://pyg.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://jbb.mhx1999.top

date +%s;  date -d @1700000000
来源：http://zjf.redwolf501.top

[R71] 日期格式化
来源：http://qfx.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oei.52xcode.cn

[R72] 等待端口就绪
来源：http://fcz.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dhr.xinyue.icu

[R73] 分割大日志
来源：http://xzo.daria6918.cn

split -l 1000 big.log part_
来源：http://hxi.yangfankeji.com

[R74] 批量重命名
来源：http://nqj.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://igi.xziqi.cn

[R75] 导出环境变量
来源：http://uvl.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://taq.bbcook.cn

[R76] 使用临时文件
来源：http://nvf.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gqr.hysaishi.cn

[R77] 读取用户输入
来源：http://muk.zhengqikj.top

read -rp "请输入: " ans
来源：http://rsy.kuanghao11.cn

[R78] 交互式菜单
来源：http://fvp.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gcq.9152youxi.cn

[R79] 解析命令行选项
来源：http://mmo.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ceh.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://xnq.aizwys.cn

time ./run.sh
来源：http://eyh.hysaishi.cn

================================================================================
来源：http://esx.gotoacloud.top

S. C / C++ 专题
来源：http://umt.316326.xyz

================================================================================
来源：http://fku.fengsongda.top

[S01] C：Hello World
来源：http://xvs.ywan-chungtsiang.top

#include <stdio.h>
来源：http://gqk.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://cdl.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://duy.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://xid.dianchejie.cn

[S03] C：读入整数
来源：http://uzd.aibaodan.cn

int x; scanf("%d", &x);
来源：http://jcw.jinghuilouyu.cn

[S04] C：字符串复制
来源：http://tus.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://jdd.aibaodan.cn

[S05] C：字符串长度
来源：http://pgj.aizwys.cn

strlen(s)
来源：http://ufz.tarul.cn

[S06] C：字符串比较
来源：http://lzb.bjfxy.top

strcmp(a, b) == 0
来源：http://uoz.hesvh.cn

[S07] C：数组遍历求和
来源：http://dkl.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://auf.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://iln.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kuh.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://fkw.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uzr.9152youxi.cn

[S10] C：指针与解引用
来源：http://qzr.epnwcf.com

int *p = &a;  *p = 5;
来源：http://uho.fengsongda.top

[S11] C：逐行读文件
来源：http://tue.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://dht.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://plx.jlsjyb.cn

fclose(f);
来源：http://vuq.ywan-chungtsiang.top

[S12] C：写文件
来源：http://rcy.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zqf.vqdsnc.cn

[S13] C：宏定义
来源：http://gna.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cgl.andypj.xyz

[S14] C：枚举
来源：http://zge.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://ufq.jlsjyb.cn

[S15] C：类型转换
来源：http://mhn.chenlongwang.top

(double) a / b
来源：http://vuc.pycfn.com

[S16] C：位操作置位
来源：http://jpz.snrcjt.cn

x |= (1 << 3);
来源：http://dhy.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://vio.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jvh.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://yii.zhixingplan.top

int main(int argc, char **argv)
来源：http://yli.yj202588.top

[S19] C：快速排序
来源：http://yji.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cdd.0kj1m.cn

[S20] C：二分查找
来源：http://onv.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hnu.guannengcc.top

[S21] C：字符类别判断
来源：http://bse.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tct.jianghu66.top

[S22] C：字符串转数字
来源：http://knd.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://ihv.sjlbkw.cn

[S23] C：随机数
来源：http://vhk.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://wrv.chenlongwang.top

[S24] C：获取本地时间
来源：http://rdl.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gok.hesvh.cn

[S25] C：内存拷贝
来源：http://xkb.zdbjq.cn

memcpy(dst, src, n);
来源：http://ayx.fehbvm.com

[S26] C：内存清零
来源：http://wba.cheryme.top

memset(a, 0, sizeof a);
来源：http://gwq.yuanzhike.top

[S27] C：定义常量
来源：http://mej.cashguo.top

const double PI = 3.14159;
来源：http://ygy.chenzaomai.com

[S28] C：静态变量
来源：http://ega.fktsv.cn

static int counter = 0;
来源：http://mzm.zdqjudy.top

[S29] C：变参函数
来源：http://lpk.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yvz.mhx1999.top

[S30] C：头文件保护
来源：http://ypp.sweek.top

#ifndef X_H
来源：http://kzc.hesvh.cn

#define X_H
来源：http://bma.zhijiandao.cn

#endif
来源：http://ihf.jinqigfzy.top

[S31] C++：Hello World
来源：http://kyq.yj20258888.top

#include <iostream>
来源：http://aqt.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://fup.xziqi.cn

[S32] C++：字符串
来源：http://phz.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://vne.redwolf501.top

[S33] C++：vector 增删
来源：http://pvf.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://psq.xinyue.icu

[S34] C++：遍历 vector
来源：http://jzx.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://hnp.tianlin.xyz


<!-- 参考信息 -->