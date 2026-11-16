代发 wailian999

[Q63] 开启事务
来源：http://lnh.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://qyo.yongpay.top

[Q64] 提交事务
来源：http://eyx.yuanzhike.top

COMMIT;
来源：http://dbd.sweek.top

[Q65] 回滚事务
来源：http://xwn.sxryk.cn

ROLLBACK;
来源：http://kxj.sxryk.cn

[Q66] 行锁查询
来源：http://wqr.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://edx.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://okw.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zjh.sweek.top

[Q68] 保存点
来源：http://izs.yvedp.cn

SAVEPOINT sp1;
来源：http://mfx.jqgufenzy.top

ROLLBACK TO sp1;
来源：http://qyu.zhengqikj.top

[Q69] 查看执行计划
来源：http://ovm.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gxv.birdmap.top

[Q70] 更新统计信息
来源：http://und.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://ilj.nwbrower.top

[Q71] 查看建表语句
来源：http://osc.jlsjyb.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://znq.zdqjudy.top

[Q72] 查看索引
来源：http://ssm.jqgfzy.top

SHOW INDEX FROM users;
来源：http://akn.gzhubu.top

[Q73] 查看表状态
来源：http://itu.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ded.mhx1999.top

[Q74] 强制使用索引
来源：http://jmj.zycfv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rvf.aizwys.cn

[Q75] 日期格式化
来源：http://ajr.yvedp.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mhf.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yme.hnqzz.top

[Q76] 按天统计
来源：http://ugd.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xwu.52xcode.cn

[Q77] 时间加减
来源：http://mbu.xuanzx.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rax.zhijiandao.cn

[Q78] 当前时间
来源：http://ceu.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lvq.gaohongyu789.top

[Q79] 字符串拼接
来源：http://zom.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jus.jinqigufen.top

[Q80] 字符串截取
来源：http://jcr.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qmq.yanxiufei.cn

[Q81] 字符串替换
来源：http://sib.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jui.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://dzd.wangdashe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yuj.yj202588.top

[Q83] 大小写转换
来源：http://los.fktsv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://isu.yuxming.cn

[Q84] 去除首尾空格
来源：http://pvp.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://tvo.cheryme.top

[Q85] 数值取整
来源：http://khk.quarkkingdee.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lxq.meibo888.top

[Q86] 读取 JSON 字段
来源：http://egx.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ngr.jiagoushi.top

[Q87] JSON 字段做条件
来源：http://skq.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gvk.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://uuc.bbcook.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wyi.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vcu.jiagoushi.top

[Q89] 判断表是否存在
来源：http://qdt.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bli.zdqjudy.top

[Q90] 生成序号列
来源：http://yjt.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://agg.pycfn.com

================================================================================
来源：http://fte.redwolf501.top

R. Bash 专题
来源：http://pyi.nanxinkj.top

================================================================================
来源：http://pqi.wangdashe.top

[R01] shebang 与严格模式
来源：http://xei.jinqigfzy.top

#!/usr/bin/env bash
来源：http://hxi.cashguo.top

set -euo pipefail
来源：http://bnv.xziqi.cn

[R02] 变量赋值与使用
来源：http://gzw.dashuyun.cn

name="Tom"; echo "$name"
来源：http://nxp.smart0.xyz

[R03] 只读变量
来源：http://fdb.sjlbkw.cn

readonly PI=3.14
来源：http://eex.fktsv.cn

[R04] 位置参数
来源：http://kjq.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cia.ydzc1.top

[R05] 参数默认值
来源：http://znz.jinqigfzy.top

name="${1:-default}"
来源：http://fyz.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://ioz.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ttc.52xcode.cn

[R07] if 判断文件
来源：http://xqu.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mfj.9152youxi.cn

[R08] 数值比较
来源：http://ksl.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://ntj.uphjek.com

[R09] 字符串比较
来源：http://imm.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hgc.tanke756.top

[R10] 正则匹配
来源：http://vpb.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lha.hywenlv.cn

[R11] case 多分支
来源：http://zwl.yj202588.top

case "$1" in
来源：http://nvt.ehwqpu.com

start) echo "启动" ;;
来源：http://phr.fzhhl.top

stop)  echo "停止" ;;
来源：http://nbv.fzhhl.top

*)     echo "未知命令" ;;
来源：http://nvx.xinyue.icu

esac
来源：http://zmx.gzhubu.top

[R12] for 遍历文件
来源：http://buk.feifeiyinyue.top

for f in *.txt; do echo "$f"; done
来源：http://xvz.hammf.cn

[R13] for 计数循环
来源：http://nvr.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://quq.epnwcf.com

[R14] C 风格 for
来源：http://brr.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pve.xziqi.cn

[R15] while 逐行读文件
来源：http://sun.hywenlv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://woy.gaohongyu789.top

[R16] until 等待条件
来源：http://toq.gogol.net.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mtp.tian-w.cn

[R17] 数组定义与取值
来源：http://eny.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://jye.xziqi.cn

[R18] 遍历数组
来源：http://mku.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://psi.mhx1999.top

[R19] 数组长度
来源：http://whh.sufxvd.cn

echo "${#arr[@]}"
来源：http://yce.sufxvd.cn

[R20] 关联数组（字典）
来源：http://ktf.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eyw.quarkkingdee.top

[R21] 字符串长度
来源：http://ypz.yuxming.cn

echo "${#s}"
来源：http://jdx.pengpengdd.cyou

[R22] 截取子串
来源：http://vvy.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://vfs.bjfxy.top

[R23] 字符串替换
来源：http://anr.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lnp.yonumen.top

[R24] 大小写转换
来源：http://gox.shangyingyoupin.top

echo "${s^^}"; echo "${s,,}"
来源：http://wgc.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://cug.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://bmc.chenzaomai.com

[R26] 命令替换
来源：http://fkq.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://ram.shangyingyoupin.top

[R27] 算术展开
来源：http://lyo.ydzc1.top

echo $((1 + 2 * 3))
来源：http://jwz.zhengqikj.top

[R28] 浮点运算
来源：http://kkl.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://lkg.gaohongyu789.top

[R29] 定义函数
来源：http://yhh.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lbl.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://lzj.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://fai.xziqi.cn

[R31] 局部变量
来源：http://dov.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://whv.chenzaomai.com

[R32] 参数个数校验
来源：http://xir.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xcn.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://ebd.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ctc.cheryme.top

[R34] 退出时清理
来源：http://ipf.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://mtb.haohaochexian.top

[R35] 后台执行并等待
来源：http://czz.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://inj.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://dby.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lwi.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://nap.tian-w.cn

files=$(ls -1)
来源：http://imy.shuidangran.top

[R38] 管道串联
来源：http://eps.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://ybg.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://giw.birdmap.top

cmd > out.log 2>&1
来源：http://jkw.meibo888.top

[R40] 追加写日志
来源：http://fxv.zhengqikj.top

echo "log" >> out.log
来源：http://ifj.yueranfly.top

[R41] 丢弃输出
来源：http://llo.316326.xyz

cmd >/dev/null 2>&1
来源：http://fui.svipenyu.cn

[R42] 输入重定向
来源：http://ufx.ybcxt.top

wc -l < a.txt
来源：http://jmr.jianghu66.top

[R43] 按名字查找文件
来源：http://ptj.hesvh.cn

find . -name "*.log" -type f
来源：http://gka.fzhhl.top

[R44] 按修改时间查找
来源：http://pfa.fehbvm.com

find . -mtime -7 -type f
来源：http://mtm.0kj1m.cn

[R45] 批量删除
来源：http://ckw.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://ofc.bjfxy.top

[R46] 递归替换文件内容
来源：http://cxr.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zrv.gzhubu.top

[R47] sed 单行替换
来源：http://leq.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://loz.ydzc1.top

[R48] awk 取指定列
来源：http://pgo.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://lev.hongshengwenyu.top

[R49] awk 带条件
来源：http://zku.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eyj.fehbvm.com

[R50] awk 求和
来源：http://mgw.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://ojk.svipenyu.cn

[R51] 排序去重取前几
来源：http://wnn.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kcc.dianchejie.cn

[R52] 统计行数
来源：http://siy.tarul.cn

wc -l a.txt
来源：http://dny.cashguo.top

[R53] 查看文件头与实时尾
来源：http://csq.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pgg.bjfxy.top

[R54] 比较两个文件
来源：http://ubz.jqgfzy.top

diff a.txt b.txt
来源：http://ssh.xziqi.cn

[R55] 压缩与解压
来源：http://wle.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eqw.aibaodan.cn

[R56] 远程拷贝
来源：http://xjz.zhiwuduotai.top

scp file user@host:/path/
来源：http://ykv.zhengqikj.top

[R57] 远程执行命令
来源：http://bbd.ppjwa.cn

ssh user@host 'uptime'
来源：http://jjx.zhaomingkeji.xyz

[R58] 下载文件
来源：http://uvi.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ual.jlsjyb.cn

[R59] 发 POST JSON
来源：http://dgq.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kjt.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://keh.aibaodan.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eva.dianchejie.cn

[R61] 磁盘占用
来源：http://roo.ehwqpu.com

df -h;  du -sh *
来源：http://ywl.iojbl.cn

[R62] 找最占空间的文件
来源：http://xbi.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://odm.jqgfzy.top

[R63] 内存与进程
来源：http://cqk.yonumen.top

free -h;  ps aux | grep nginx
来源：http://gmj.xuetiantiany.cn

[R64] 结束进程
来源：http://rol.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://kdg.feifeiyinyue.top

[R65] 查看端口占用
来源：http://gnd.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xgy.shanyushiyangtech.top

[R66] 定时任务
来源：http://evu.svipenyu.cn

crontab -e;  crontab -l
来源：http://rdu.vqdsnc.cn

[R67] 生成随机十六进制串
来源：http://xje.shzxlz.cn

openssl rand -hex 16
来源：http://eku.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://eym.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rpr.ppjwa.cn

[R69] 生成随机密码
来源：http://esw.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://fub.gotoacloud.top

[R70] 时间戳与互转
来源：http://rgi.uphjek.com

date +%s;  date -d @1700000000
来源：http://qdl.jianghu66.top

[R71] 日期格式化
来源：http://wym.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kti.yj20258.top

[R72] 等待端口就绪
来源：http://bkc.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://knt.sxryk.cn

[R73] 分割大日志
来源：http://qem.daxiang520.top

split -l 1000 big.log part_
来源：http://ykz.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://dmf.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rda.jqgfzy.top

[R75] 导出环境变量
来源：http://lph.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://mtq.gogol.net.cn

[R76] 使用临时文件
来源：http://lat.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yde.bbcook.cn

[R77] 读取用户输入
来源：http://pha.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://rza.tian-w.cn

[R78] 交互式菜单
来源：http://zze.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://omk.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://czf.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://glh.tanke756.top

[R80] 查看脚本执行耗时
来源：http://pnk.zhoulong.xyz

time ./run.sh
来源：http://fla.yueranfly.top

================================================================================
来源：http://ijc.aizwys.cn

S. C / C++ 专题
来源：http://ibx.feifeiyinyue.top

================================================================================
来源：http://cvw.xziqi.cn

[S01] C：Hello World
来源：http://rng.svipenyu.cn

#include <stdio.h>
来源：http://bhh.sxryk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pxh.mhx1999.top

[S02] C：变量与格式化输出
来源：http://rsi.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://sek.jlsjyb.cn

[S03] C：读入整数
来源：http://iyq.ehwqpu.com

int x; scanf("%d", &x);
来源：http://gnf.yonumen.top

[S04] C：字符串复制
来源：http://efl.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://mgg.wangshuangyany.cn

[S05] C：字符串长度
来源：http://ihh.zhijiandao.cn

strlen(s)
来源：http://uhc.vehdjk.com

[S06] C：字符串比较
来源：http://ehn.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://kam.jinqigufen.top

[S07] C：数组遍历求和
来源：http://edq.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://esw.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://equ.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zbd.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://jmq.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://twm.hcnkem.com

[S10] C：指针与解引用
来源：http://axl.bbcook.cn

int *p = &a;  *p = 5;
来源：http://szx.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://xqy.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://lzs.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fki.daxiang520.top

fclose(f);
来源：http://dmh.svipenyu.cn

[S12] C：写文件
来源：http://pwl.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bqs.fanxiaobao.xyz

[S13] C：宏定义
来源：http://pvt.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tzi.jyoumei.cn

[S14] C：枚举
来源：http://nwq.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://fxt.mhx1999.top

[S15] C：类型转换
来源：http://slu.zhiwuduotai.top

(double) a / b
来源：http://amj.zhixingplan.top

[S16] C：位操作置位
来源：http://wux.zhongyouzk.top

x |= (1 << 3);
来源：http://cqy.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://ruy.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bpk.yanxiufei.cn

[S18] C：命令行参数
来源：http://lbm.xuanzx.com

int main(int argc, char **argv)
来源：http://ctv.chenlongwang.top

[S19] C：快速排序
来源：http://uqw.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://ihw.guowangkeji.top

[S20] C：二分查找
来源：http://sva.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jvg.jinqigufen.top

[S21] C：字符类别判断
来源：http://wth.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zbf.haohaochexian.top

[S22] C：字符串转数字
来源：http://qsk.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://ewt.haohaochexian.top

[S23] C：随机数
来源：http://vxj.yongpay.top

srand(time(NULL));  int r = rand() % 100;
来源：http://etf.yangfankeji.com

[S24] C：获取本地时间
来源：http://ljc.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jhe.zhixingplan.top

[S25] C：内存拷贝
来源：http://mdl.tarul.cn

memcpy(dst, src, n);
来源：http://llb.zhongyouzk.top

[S26] C：内存清零
来源：http://fer.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://jxs.havefunace.top

[S27] C：定义常量
来源：http://xqv.ivvv.top

const double PI = 3.14159;
来源：http://wyp.jqgufenzy.top

[S28] C：静态变量
来源：http://hgz.yj20258888.top

static int counter = 0;
来源：http://hlh.jiagoushi.top

[S29] C：变参函数
来源：http://bmp.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://afo.jinqigufen.top

[S30] C：头文件保护
来源：http://hyp.quarkkingdee.top

#ifndef X_H
来源：http://wtz.fzhhl.top

#define X_H
来源：http://yuw.yanxiufei.cn

#endif
来源：http://igb.zhengqikj.top

[S31] C++：Hello World
来源：http://kkk.ydjk.org.cn

#include <iostream>
来源：http://cra.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://wjm.birdmap.top

[S32] C++：字符串
来源：http://tvw.cashguo.top

std::string s = "hi";  s += "!";
来源：http://diy.zycfv.cn


<!-- 参考信息 -->