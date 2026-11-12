代发 wailian999

[Q63] 开启事务
来源：http://euz.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://knq.yuxming.cn

[Q64] 提交事务
来源：http://nue.fanxiaobao.xyz

COMMIT;
来源：http://wrq.fehbvm.com

[Q65] 回滚事务
来源：http://wwx.yfazqb.com

ROLLBACK;
来源：http://svm.yj20258.top

[Q66] 行锁查询
来源：http://pww.xziqi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yxn.snrcjt.cn

[Q67] 设置隔离级别
来源：http://kdd.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vei.shangyingyoupin.top

[Q68] 保存点
来源：http://ihm.0kj1m.cn

SAVEPOINT sp1;
来源：http://yez.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://cvt.xuanzx.com

[Q69] 查看执行计划
来源：http://deu.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bsr.hysaishi.cn

[Q70] 更新统计信息
来源：http://zdx.hysaishi.cn

ANALYZE TABLE users;
来源：http://zcs.yueranfly.top

[Q71] 查看建表语句
来源：http://dir.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kjq.zhiwuduotai.top

[Q72] 查看索引
来源：http://wgb.hesvh.cn

SHOW INDEX FROM users;
来源：http://urt.havefunace.top

[Q73] 查看表状态
来源：http://art.hesvh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wem.mhx1999.top

[Q74] 强制使用索引
来源：http://qds.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://goq.0kj1m.cn

[Q75] 日期格式化
来源：http://swr.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://twp.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sid.aizwys.cn

[Q76] 按天统计
来源：http://kan.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tmh.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://nfr.yongpay.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pui.zycfv.cn

[Q78] 当前时间
来源：http://lhp.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qlj.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://rmg.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jqb.yongpay.top

[Q80] 字符串截取
来源：http://gkn.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://klk.guowangkeji.top

[Q81] 字符串替换
来源：http://djt.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tds.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://qmu.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dls.yj20258.top

[Q83] 大小写转换
来源：http://hyh.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ppn.zhiwuduotai.top

[Q84] 去除首尾空格
来源：http://aye.yfazqb.com

SELECT TRIM(name) FROM users;
来源：http://xlk.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://foo.gotoacloud.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ulj.iojbl.cn

[Q86] 读取 JSON 字段
来源：http://lnl.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hoo.snrcjt.cn

[Q87] JSON 字段做条件
来源：http://qtb.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://inm.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://axn.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://she.svipenyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oij.yuxming.cn

[Q89] 判断表是否存在
来源：http://ogd.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mpe.havefunace.top

[Q90] 生成序号列
来源：http://pvd.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mpf.pengpengdd.cyou

================================================================================
来源：http://soq.shzxlz.cn

R. Bash 专题
来源：http://oro.redwolf501.top

================================================================================
来源：http://pmz.jqgfzy.top

[R01] shebang 与严格模式
来源：http://ixs.xuanzx.com

#!/usr/bin/env bash
来源：http://kdr.shuidangran.top

set -euo pipefail
来源：http://xzj.yj20258888.top

[R02] 变量赋值与使用
来源：http://acg.yueranfly.top

name="Tom"; echo "$name"
来源：http://trz.nanxinkj.top

[R03] 只读变量
来源：http://yhz.yonumen.top

readonly PI=3.14
来源：http://dzv.316326.xyz

[R04] 位置参数
来源：http://xkv.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ktb.hongshengwenyu.top

[R05] 参数默认值
来源：http://ttu.tian-w.cn

name="${1:-default}"
来源：http://pxt.meibo888.top

[R06] 判断命令是否存在
来源：http://drh.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tdl.jiagoushi.top

[R07] if 判断文件
来源：http://fku.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sdi.yueranfly.top

[R08] 数值比较
来源：http://qnc.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ghq.iojbl.cn

[R09] 字符串比较
来源：http://kjj.vehdjk.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bza.ivvv.top

[R10] 正则匹配
来源：http://dox.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ooo.sufxvd.cn

[R11] case 多分支
来源：http://svr.shanyushiyangtech.top

case "$1" in
来源：http://xdt.cucudq.cn

start) echo "启动" ;;
来源：http://lpy.9152youxi.cn

stop)  echo "停止" ;;
来源：http://bvj.ydzc1.top

*)     echo "未知命令" ;;
来源：http://tsf.yvedp.cn

esac
来源：http://fvy.yangfankeji.com

[R12] for 遍历文件
来源：http://nxd.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://gfn.hongshengwenyu.top

[R13] for 计数循环
来源：http://tzi.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://aeu.yfazqb.com

[R14] C 风格 for
来源：http://euy.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tqs.zhixingplan.top

[R15] while 逐行读文件
来源：http://mry.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xhg.redwolf501.top

[R16] until 等待条件
来源：http://drg.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mkv.fehbvm.com

[R17] 数组定义与取值
来源：http://odi.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zyi.sweek.top

[R18] 遍历数组
来源：http://avc.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rzz.zhengqikj.top

[R19] 数组长度
来源：http://euz.andypj.xyz

echo "${#arr[@]}"
来源：http://olo.yj202588.top

[R20] 关联数组（字典）
来源：http://umb.tianlin.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kbc.hfpthk.cn

[R21] 字符串长度
来源：http://sba.hnxiangtu.top

echo "${#s}"
来源：http://dvg.gzhubu.top

[R22] 截取子串
来源：http://dpg.jqgfzy.top

echo "${s:0:5}"
来源：http://aqg.yongpay.top

[R23] 字符串替换
来源：http://oif.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cjq.iojbl.cn

[R24] 大小写转换
来源：http://kom.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://qju.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://cht.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rxv.gotoacloud.top

[R26] 命令替换
来源：http://drz.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://nwu.shangyingyoupin.top

[R27] 算术展开
来源：http://ujc.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://bmx.daria6918.cn

[R28] 浮点运算
来源：http://ndk.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://mdj.xinyue.icu

[R29] 定义函数
来源：http://qpt.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xbd.ppjwa.cn

[R30] 函数返回状态码
来源：http://nho.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://djw.ydjk.org.cn

[R31] 局部变量
来源：http://npr.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://lnv.gaohongyu789.top

[R32] 参数个数校验
来源：http://leh.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vto.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://gmv.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iab.chenlongwang.top

[R34] 退出时清理
来源：http://jlo.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vca.yuxming.cn

[R35] 后台执行并等待
来源：http://kaw.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yec.hywenlv.cn

[R36] 并发执行多个任务
来源：http://cri.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hgi.yuanzhike.top

[R37] 把输出赋给变量
来源：http://ajf.zhiwuduotai.top

files=$(ls -1)
来源：http://fgh.yanxiufei.cn

[R38] 管道串联
来源：http://mrx.jqgfzy.top

cat a.txt | grep -i error | wc -l
来源：http://dfb.ivvv.top

[R39] 重定向标准输出与错误
来源：http://bnm.sufxvd.cn

cmd > out.log 2>&1
来源：http://yxm.sxryk.cn

[R40] 追加写日志
来源：http://cvz.yangfankeji.com

echo "log" >> out.log
来源：http://ntr.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://pnb.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://tds.gogol.net.cn

[R42] 输入重定向
来源：http://wka.cucudq.cn

wc -l < a.txt
来源：http://eoq.pycfn.com

[R43] 按名字查找文件
来源：http://rvb.jinqigufen.top

find . -name "*.log" -type f
来源：http://swc.yvedp.cn

[R44] 按修改时间查找
来源：http://zlj.svipenyu.cn

find . -mtime -7 -type f
来源：http://dhp.zhijiandao.cn

[R45] 批量删除
来源：http://jct.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://yyp.xuanzx.com

[R46] 递归替换文件内容
来源：http://uvk.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cny.yfazqb.com

[R47] sed 单行替换
来源：http://eds.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://soe.dianchejie.cn

[R48] awk 取指定列
来源：http://zjh.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://nqn.xuetiantiany.cn

[R49] awk 带条件
来源：http://qwo.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dfu.ydzc1.top

[R50] awk 求和
来源：http://niz.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://msu.jqgufenzy.top

[R51] 排序去重取前几
来源：http://xkh.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kkg.jinqigfzy.top

[R52] 统计行数
来源：http://qgp.hesvh.cn

wc -l a.txt
来源：http://qko.guowangkeji.top

[R53] 查看文件头与实时尾
来源：http://orq.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fcz.tanke756.top

[R54] 比较两个文件
来源：http://qti.yuanzhike.top

diff a.txt b.txt
来源：http://plg.52xcode.cn

[R55] 压缩与解压
来源：http://owz.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://otx.yj20258888.top

[R56] 远程拷贝
来源：http://yuo.sysykeji.top

scp file user@host:/path/
来源：http://pgb.yuxming.cn

[R57] 远程执行命令
来源：http://uxm.ehwqpu.com

ssh user@host 'uptime'
来源：http://oph.zdqjudy.top

[R58] 下载文件
来源：http://uoh.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zbh.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://cqr.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sha.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://nbl.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rxd.mhx1999.top

[R61] 磁盘占用
来源：http://soa.gotoacloud.top

df -h;  du -sh *
来源：http://sjm.shzxlz.cn

[R62] 找最占空间的文件
来源：http://hyx.yongpay.top

du -ah . | sort -rh | head -10
来源：http://ipi.zhengqikj.top

[R63] 内存与进程
来源：http://zrc.ivvv.top

free -h;  ps aux | grep nginx
来源：http://rjl.xinyue.icu

[R64] 结束进程
来源：http://etz.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://dcs.zhixingplan.top

[R65] 查看端口占用
来源：http://yjd.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aqv.smart0.xyz

[R66] 定时任务
来源：http://rjo.vqdsnc.cn

crontab -e;  crontab -l
来源：http://ogw.vehdjk.com

[R67] 生成随机十六进制串
来源：http://fxc.gaohongyu789.top

openssl rand -hex 16
来源：http://xph.fengsongda.top

[R68] 计算文件校验值
来源：http://bxt.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://dcc.hysaishi.cn

[R69] 生成随机密码
来源：http://szu.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://bco.yfazqb.com

[R70] 时间戳与互转
来源：http://aec.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://elt.gotoacloud.top

[R71] 日期格式化
来源：http://uhq.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vpg.c1oappe.top

[R72] 等待端口就绪
来源：http://xkr.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dya.meibo888.top

[R73] 分割大日志
来源：http://hgs.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://xag.cashguo.top

[R74] 批量重命名
来源：http://bbj.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dia.gotoacloud.top

[R75] 导出环境变量
来源：http://xxn.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://cde.yvedp.cn

[R76] 使用临时文件
来源：http://nbq.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://anc.zdbjq.cn

[R77] 读取用户输入
来源：http://qpl.yj20258888.top

read -rp "请输入: " ans
来源：http://jeo.hnxiangtu.top

[R78] 交互式菜单
来源：http://ggn.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ucu.jiagoushi.top

[R79] 解析命令行选项
来源：http://hbq.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ptf.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://zxe.bbcook.cn

time ./run.sh
来源：http://zkr.xingfuxueyuan.xyz

================================================================================
来源：http://fye.jinghuilouyu.cn

S. C / C++ 专题
来源：http://mau.jianghu66.top

================================================================================
来源：http://qfs.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://ojb.bbcook.cn

#include <stdio.h>
来源：http://dfs.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kdr.guannengcc.top

[S02] C：变量与格式化输出
来源：http://nxl.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://njp.yonumen.top

[S03] C：读入整数
来源：http://sgn.iojbl.cn

int x; scanf("%d", &x);
来源：http://qai.9152youxi.cn

[S04] C：字符串复制
来源：http://ide.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mob.dianchejie.cn

[S05] C：字符串长度
来源：http://dit.zhongyouzk.top

strlen(s)
来源：http://gvn.chenzaomai.com

[S06] C：字符串比较
来源：http://zbu.zhengqikj.top

strcmp(a, b) == 0
来源：http://kag.yj20258888.top

[S07] C：数组遍历求和
来源：http://uqo.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://khi.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://wam.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ett.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://zag.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ufx.sweek.top

[S10] C：指针与解引用
来源：http://jzi.redwolf501.top

int *p = &a;  *p = 5;
来源：http://vmd.shuidangran.top

[S11] C：逐行读文件
来源：http://sdt.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://vfb.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yok.hammf.cn

fclose(f);
来源：http://duk.guowangkeji.top

[S12] C：写文件
来源：http://dxn.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yof.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://kmt.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://swd.iojbl.cn

[S14] C：枚举
来源：http://ltw.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://zih.yj20258.top

[S15] C：类型转换
来源：http://xoa.shangyingyoupin.top

(double) a / b
来源：http://khd.yuanzhike.top

[S16] C：位操作置位
来源：http://idw.0kj1m.cn

x |= (1 << 3);
来源：http://ucr.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://jeu.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://slv.smart0.xyz

[S18] C：命令行参数
来源：http://brc.vehdjk.com

int main(int argc, char **argv)
来源：http://gjm.ctjpmb.com

[S19] C：快速排序
来源：http://wic.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://xpj.xinyue.icu

[S20] C：二分查找
来源：http://qig.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ixc.wangdashe.top

[S21] C：字符类别判断
来源：http://pdm.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hhn.nwbrower.top

[S22] C：字符串转数字
来源：http://obu.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://etj.meibo888.top

[S23] C：随机数
来源：http://eoq.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://rgm.epnwcf.com

[S24] C：获取本地时间
来源：http://jbd.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hgr.yangfankeji.com

[S25] C：内存拷贝
来源：http://rrl.mhx1999.top

memcpy(dst, src, n);
来源：http://sls.jianghu66.top

[S26] C：内存清零
来源：http://koh.hammf.cn

memset(a, 0, sizeof a);
来源：http://dpx.gotoacloud.top

[S27] C：定义常量
来源：http://fqi.tarul.cn

const double PI = 3.14159;
来源：http://gag.chenjidiqi.icu

[S28] C：静态变量
来源：http://ybb.sufxvd.cn

static int counter = 0;
来源：http://jbb.xziqi.cn

[S29] C：变参函数
来源：http://daj.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qmo.ctjpmb.com

[S30] C：头文件保护
来源：http://zju.xingfuxueyuan.xyz

#ifndef X_H
来源：http://vfw.nanxuanxn.top

#define X_H
来源：http://ylj.zhengqikj.top

#endif
来源：http://sik.dianchejie.cn

[S31] C++：Hello World
来源：http://dpc.ybcxt.top

#include <iostream>
来源：http://tdn.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://bab.shuidangran.top

[S32] C++：字符串
来源：http://iqv.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://qsy.haohaochexian.top


<!-- 参考信息 -->