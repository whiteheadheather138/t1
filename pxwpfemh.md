代发 wailian999

[Q65] 回滚事务
来源：http://yts.xylfe.cn

ROLLBACK;
来源：http://jea.gogol.net.cn

[Q66] 行锁查询
来源：http://jdf.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ico.zdbjq.cn

[Q67] 设置隔离级别
来源：http://mig.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fvd.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://gha.yuanzhike.top

SAVEPOINT sp1;
来源：http://xkn.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://sdu.cashguo.top

[Q69] 查看执行计划
来源：http://fjo.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pkp.snrcjt.cn

[Q70] 更新统计信息
来源：http://som.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://xrd.ivvv.top

[Q71] 查看建表语句
来源：http://iej.52xcode.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fgu.chenzaomai.com

[Q72] 查看索引
来源：http://ffk.nanxinkj.top

SHOW INDEX FROM users;
来源：http://gdd.feifeiyinyue.top

[Q73] 查看表状态
来源：http://ggd.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://gzo.vehdjk.com

[Q74] 强制使用索引
来源：http://krr.tian-w.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://szr.jyoumei.cn

[Q75] 日期格式化
来源：http://zuy.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lir.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rsv.smart0.xyz

[Q76] 按天统计
来源：http://mfv.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fpb.chenzaomai.com

[Q77] 时间加减
来源：http://lti.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tvh.dianchejie.cn

[Q78] 当前时间
来源：http://lfr.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kuv.xuanzx.com

[Q79] 字符串拼接
来源：http://iso.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://duf.cqqwz.cn

[Q80] 字符串截取
来源：http://wux.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mdx.dashuyun.cn

[Q81] 字符串替换
来源：http://xlo.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kvt.pycfn.com

[Q82] 字符长度与字节长度
来源：http://xrv.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kod.jiagoushi.top

[Q83] 大小写转换
来源：http://dme.gzhubu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pzn.zycfv.cn

[Q84] 去除首尾空格
来源：http://gdw.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://ohj.daxiang520.top

[Q85] 数值取整
来源：http://yae.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eqy.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://kjq.xziqi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zdf.sysykeji.top

[Q87] JSON 字段做条件
来源：http://tab.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nds.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://rvm.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hgh.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pua.aizwys.cn

[Q89] 判断表是否存在
来源：http://qcc.ydzc1.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fha.gotoacloud.top

[Q90] 生成序号列
来源：http://qwe.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lmd.cdnleiting.top

================================================================================
来源：http://uyd.nanxinkj.top

R. Bash 专题
来源：http://ntq.shuidangran.top

================================================================================
来源：http://xfs.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://wrs.zdbjq.cn

#!/usr/bin/env bash
来源：http://vtk.sjlbkw.cn

set -euo pipefail
来源：http://bbo.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://eul.xziqi.cn

name="Tom"; echo "$name"
来源：http://xxf.pengpengdd.cyou

[R03] 只读变量
来源：http://bjg.zhoulong.xyz

readonly PI=3.14
来源：http://mqn.tian-w.cn

[R04] 位置参数
来源：http://jdu.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rsl.xylfe.cn

[R05] 参数默认值
来源：http://pry.cashguo.top

name="${1:-default}"
来源：http://log.jianghu66.top

[R06] 判断命令是否存在
来源：http://kmx.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dxz.gzhubu.top

[R07] if 判断文件
来源：http://ebz.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ipx.shzxlz.cn

[R08] 数值比较
来源：http://sar.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://wvw.guannengcc.top

[R09] 字符串比较
来源：http://zol.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://umz.jinqigfzy.top

[R10] 正则匹配
来源：http://hfx.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ggy.birdmap.top

[R11] case 多分支
来源：http://ewg.hnqzz.top

case "$1" in
来源：http://jna.cucudq.cn

start) echo "启动" ;;
来源：http://sea.ydzc1.top

stop)  echo "停止" ;;
来源：http://ghz.andypj.xyz

*)     echo "未知命令" ;;
来源：http://jrz.feifeiyinyue.top

esac
来源：http://oyw.xylfe.cn

[R12] for 遍历文件
来源：http://fsv.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://jhi.cdnleiting.top

[R13] for 计数循环
来源：http://tea.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://yky.tian-w.cn

[R14] C 风格 for
来源：http://eew.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qqf.daria6918.cn

[R15] while 逐行读文件
来源：http://lhn.xziqi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bsj.jinqigfzy.top

[R16] until 等待条件
来源：http://kbz.hysaishi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oww.hfpthk.cn

[R17] 数组定义与取值
来源：http://ppd.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://pjs.shuidangran.top

[R18] 遍历数组
来源：http://yxo.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qfd.quarkkingdee.top

[R19] 数组长度
来源：http://dqw.cucudq.cn

echo "${#arr[@]}"
来源：http://cvt.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://gto.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zda.52xcode.cn

[R21] 字符串长度
来源：http://yye.cqqwz.cn

echo "${#s}"
来源：http://wsh.0kj1m.cn

[R22] 截取子串
来源：http://cfm.wangdashe.top

echo "${s:0:5}"
来源：http://tgw.nwbrower.top

[R23] 字符串替换
来源：http://pqw.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rju.svipenyu.cn

[R24] 大小写转换
来源：http://lwh.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bbn.daria6918.cn

[R25] 去后缀 / 去前缀
来源：http://jot.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lfb.jianghu66.top

[R26] 命令替换
来源：http://sdz.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://syi.yvedp.cn

[R27] 算术展开
来源：http://agl.redwolf501.top

echo $((1 + 2 * 3))
来源：http://ldz.kuanghao11.cn

[R28] 浮点运算
来源：http://lcb.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://clk.zdqjudy.top

[R29] 定义函数
来源：http://krv.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qfd.pycfn.com

[R30] 函数返回状态码
来源：http://wiq.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://mrx.bbcook.cn

[R31] 局部变量
来源：http://lsn.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://cqj.gzhubu.top

[R32] 参数个数校验
来源：http://ydw.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://shi.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://myh.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vze.vehdjk.com

[R34] 退出时清理
来源：http://xqp.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://eoi.snrcjt.cn

[R35] 后台执行并等待
来源：http://ewz.ctjpmb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://yqs.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://nxn.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bph.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://rpn.sxryk.cn

files=$(ls -1)
来源：http://wiu.yj202588.top

[R38] 管道串联
来源：http://daa.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://avn.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://joz.hesvh.cn

cmd > out.log 2>&1
来源：http://uiz.gaohongyu789.top

[R40] 追加写日志
来源：http://mqk.sysykeji.top

echo "log" >> out.log
来源：http://fjm.zdqjudy.top

[R41] 丢弃输出
来源：http://cgo.redwolf501.top

cmd >/dev/null 2>&1
来源：http://qau.xuanzx.com

[R42] 输入重定向
来源：http://gve.shangyingyoupin.top

wc -l < a.txt
来源：http://ebe.gotoacloud.top

[R43] 按名字查找文件
来源：http://oiy.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://osa.9152youxi.cn

[R44] 按修改时间查找
来源：http://agw.jinqigufen.top

find . -mtime -7 -type f
来源：http://eno.chenlongwang.top

[R45] 批量删除
来源：http://lnz.cashguo.top

find . -name "*.tmp" -delete
来源：http://trw.yfazqb.com

[R46] 递归替换文件内容
来源：http://qzc.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://luu.mhx1999.top

[R47] sed 单行替换
来源：http://vhp.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ycm.yj20258.top

[R48] awk 取指定列
来源：http://yoy.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://ggy.redwolf501.top

[R49] awk 带条件
来源：http://qkh.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nmx.aizwys.cn

[R50] awk 求和
来源：http://ynl.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://szk.316326.xyz

[R51] 排序去重取前几
来源：http://box.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gyr.jinghuilouyu.cn

[R52] 统计行数
来源：http://acy.guowangkeji.top

wc -l a.txt
来源：http://yql.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://zys.c1oappe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sds.vqdsnc.cn

[R54] 比较两个文件
来源：http://hxb.ydjk.org.cn

diff a.txt b.txt
来源：http://ugh.yueranfly.top

[R55] 压缩与解压
来源：http://puw.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://buc.redwolf501.top

[R56] 远程拷贝
来源：http://qbo.zhongyouzk.top

scp file user@host:/path/
来源：http://onk.ydzc1.top

[R57] 远程执行命令
来源：http://fyk.sjlbkw.cn

ssh user@host 'uptime'
来源：http://rii.yanxiufei.cn

[R58] 下载文件
来源：http://fyy.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://caw.jiagoushi.top

[R59] 发 POST JSON
来源：http://qqu.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://psv.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://dfq.shanyushiyangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nra.shzxlz.cn

[R61] 磁盘占用
来源：http://hea.chenjidiqi.icu

df -h;  du -sh *
来源：http://ovj.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://sab.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://fbi.sweek.top

[R63] 内存与进程
来源：http://dso.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://cxf.daria6918.cn

[R64] 结束进程
来源：http://bdi.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://giv.chenlongwang.top

[R65] 查看端口占用
来源：http://eyb.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rke.jyoumei.cn

[R66] 定时任务
来源：http://wyb.zhongyouzk.top

crontab -e;  crontab -l
来源：http://knc.yfazqb.com

[R67] 生成随机十六进制串
来源：http://jav.ppjwa.cn

openssl rand -hex 16
来源：http://boc.iojbl.cn

[R68] 计算文件校验值
来源：http://ymq.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://yny.chenlongwang.top

[R69] 生成随机密码
来源：http://bhz.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://zeo.hysaishi.cn

[R70] 时间戳与互转
来源：http://zvu.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://biv.jyoumei.cn

[R71] 日期格式化
来源：http://kke.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://kta.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://okh.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://snw.ydzc1.top

[R73] 分割大日志
来源：http://moz.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://dat.guannengcc.top

[R74] 批量重命名
来源：http://awy.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kxn.jinqigfzy.top

[R75] 导出环境变量
来源：http://ony.guannengcc.top

export PATH="$HOME/bin:$PATH"
来源：http://ync.aibaodan.cn

[R76] 使用临时文件
来源：http://owp.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zoq.xziqi.cn

[R77] 读取用户输入
来源：http://vkm.bbcook.cn

read -rp "请输入: " ans
来源：http://kml.tarul.cn

[R78] 交互式菜单
来源：http://zei.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ggu.0kj1m.cn

[R79] 解析命令行选项
来源：http://fdr.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://flq.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://wwt.shangyingyoupin.top

time ./run.sh
来源：http://bmo.chenzaomai.com

================================================================================
来源：http://vcb.gogol.net.cn

S. C / C++ 专题
来源：http://qzp.shanyushiyangkeji.top

================================================================================
来源：http://wha.jlsjyb.cn

[S01] C：Hello World
来源：http://xvf.tian-w.cn

#include <stdio.h>
来源：http://pao.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://onb.yj20258.top

[S02] C：变量与格式化输出
来源：http://owz.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://xzu.hammf.cn

[S03] C：读入整数
来源：http://vfh.fktsv.cn

int x; scanf("%d", &x);
来源：http://pyz.xinyue.icu

[S04] C：字符串复制
来源：http://cqb.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://ljm.fehbvm.com

[S05] C：字符串长度
来源：http://bwc.sysykeji.top

strlen(s)
来源：http://tlx.aibaodan.cn

[S06] C：字符串比较
来源：http://jkh.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://eav.ppjwa.cn

[S07] C：数组遍历求和
来源：http://eyq.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ydc.yj20258.top

[S08] C：动态内存分配与释放
来源：http://etc.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uca.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://mdp.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ddm.quarkkingdee.top

[S10] C：指针与解引用
来源：http://fns.epnwcf.com

int *p = &a;  *p = 5;
来源：http://exa.quarkkingdee.top

[S11] C：逐行读文件
来源：http://onn.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://iso.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ixz.nanxinkj.top

fclose(f);
来源：http://usn.sxryk.cn

[S12] C：写文件
来源：http://jvt.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mco.sysykeji.top

[S13] C：宏定义
来源：http://ixn.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rbp.wangdashe.top

[S14] C：枚举
来源：http://iey.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://flw.ydzc1.top

[S15] C：类型转换
来源：http://fvu.zhoulong.xyz

(double) a / b
来源：http://fbe.aizwys.cn

[S16] C：位操作置位
来源：http://jrp.zdqjudy.top

x |= (1 << 3);
来源：http://fgn.ivvv.top

[S17] C：安全拼接字符串
来源：http://xel.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jxe.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://vys.yongpay.top

int main(int argc, char **argv)
来源：http://hsa.jyoumei.cn

[S19] C：快速排序
来源：http://nes.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://eaa.xuetiantiany.cn

[S20] C：二分查找
来源：http://szf.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nea.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://hso.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jze.yvedp.cn

[S22] C：字符串转数字
来源：http://qmf.nwbrower.top

atoi("42");  strtod("3.14", NULL);
来源：http://oqo.dashuyun.cn

[S23] C：随机数
来源：http://upe.hcnkem.com

srand(time(NULL));  int r = rand() % 100;
来源：http://abm.hammf.cn

[S24] C：获取本地时间
来源：http://bag.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lej.yj20258.top

[S25] C：内存拷贝
来源：http://auj.jqgufenzy.top

memcpy(dst, src, n);
来源：http://qyg.shzxlz.cn

[S26] C：内存清零
来源：http://gdd.tanke756.top

memset(a, 0, sizeof a);
来源：http://lpo.vehdjk.com

[S27] C：定义常量
来源：http://xdu.cqqwz.cn

const double PI = 3.14159;
来源：http://gkr.yonumen.top

[S28] C：静态变量
来源：http://ytb.sufxvd.cn

static int counter = 0;
来源：http://gtb.dashuyun.cn

[S29] C：变参函数
来源：http://mbz.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hpa.jqgfzy.top

[S30] C：头文件保护
来源：http://vdh.ywan-chungtsiang.top

#ifndef X_H
来源：http://blf.hnxiangtu.top

#define X_H
来源：http://duq.jiagoushi.top

#endif
来源：http://hka.xinyue.icu

[S31] C++：Hello World
来源：http://dsj.cheryme.top

#include <iostream>
来源：http://hqg.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://yho.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://vwj.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://aby.hysaishi.cn

[S33] C++：vector 增删
来源：http://vfd.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://olw.guowangkeji.top

[S34] C++：遍历 vector
来源：http://rbk.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://vab.hfpthk.cn


<!-- 参考信息 -->