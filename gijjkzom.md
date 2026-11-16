代发 wailian999

[Q61] 移动平均
来源：http://spy.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://peh.sjlbkw.cn

[Q62] 分组占比
来源：http://jvx.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bak.pengpengdd.cyou

[Q63] 开启事务
来源：http://njs.xuanzx.com

START TRANSACTION;                -- 或 BEGIN
来源：http://fzn.vehdjk.com

[Q64] 提交事务
来源：http://vqb.shangyingyoupin.top

COMMIT;
来源：http://eeh.shangyingyoupin.top

[Q65] 回滚事务
来源：http://app.xingfuxueyuan.xyz

ROLLBACK;
来源：http://nmw.bjfxy.top

[Q66] 行锁查询
来源：http://ayt.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mkh.yuanzhike.top

[Q67] 设置隔离级别
来源：http://drt.wangshuangyany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oua.dianchejie.cn

[Q68] 保存点
来源：http://znb.yvedp.cn

SAVEPOINT sp1;
来源：http://hnp.guowangkeji.top

ROLLBACK TO sp1;
来源：http://bei.yj20258888.top

[Q69] 查看执行计划
来源：http://yaw.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wjz.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://xhb.yj20258.top

ANALYZE TABLE users;
来源：http://ezs.smart0.xyz

[Q71] 查看建表语句
来源：http://nea.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ofm.kuanghao11.cn

[Q72] 查看索引
来源：http://vks.quarkkingdee.top

SHOW INDEX FROM users;
来源：http://yos.cqqwz.cn

[Q73] 查看表状态
来源：http://sut.mhx1999.top

SHOW TABLE STATUS LIKE 'users';
来源：http://bck.feifeiyinyue.top

[Q74] 强制使用索引
来源：http://idp.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gdp.haohaochexian.top

[Q75] 日期格式化
来源：http://tks.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://emu.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dcl.jiagoushi.top

[Q76] 按天统计
来源：http://zyt.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://upn.zhoulong.xyz

[Q77] 时间加减
来源：http://qdn.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nuo.bbcook.cn

[Q78] 当前时间
来源：http://aey.feifeiyinyue.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nei.gogol.net.cn

[Q79] 字符串拼接
来源：http://zju.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ild.kuanghao11.cn

[Q80] 字符串截取
来源：http://ebg.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aqr.snrcjt.cn

[Q81] 字符串替换
来源：http://vii.hfpthk.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gqm.tarul.cn

[Q82] 字符长度与字节长度
来源：http://xiz.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pnf.feifeiyinyue.top

[Q83] 大小写转换
来源：http://wxw.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hma.jqgfzy.top

[Q84] 去除首尾空格
来源：http://wxq.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://kow.mhx1999.top

[Q85] 数值取整
来源：http://orj.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://osa.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://ihg.hfpthk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pzp.hfpthk.cn

[Q87] JSON 字段做条件
来源：http://lte.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://phs.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://mqo.svipenyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vym.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oui.jinqigfzy.top

[Q89] 判断表是否存在
来源：http://tkf.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xlm.xinyue.icu

[Q90] 生成序号列
来源：http://iys.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aqa.52xcode.cn

================================================================================
来源：http://uao.xuanzx.com

R. Bash 专题
来源：http://qvj.cdnleiting.top

================================================================================
来源：http://jdm.ybcxt.top

[R01] shebang 与严格模式
来源：http://fpz.dashuyun.cn

#!/usr/bin/env bash
来源：http://lzc.zhiwuduotai.top

set -euo pipefail
来源：http://ljk.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://itk.fengsongda.top

name="Tom"; echo "$name"
来源：http://hto.zhiwuduotai.top

[R03] 只读变量
来源：http://xwh.jyoumei.cn

readonly PI=3.14
来源：http://apj.zdqjudy.top

[R04] 位置参数
来源：http://gfo.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bgt.xinyue.icu

[R05] 参数默认值
来源：http://gqx.daria6918.cn

name="${1:-default}"
来源：http://czg.yonumen.top

[R06] 判断命令是否存在
来源：http://rcy.wangdashe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yvh.yfazqb.com

[R07] if 判断文件
来源：http://ncn.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zmv.xziqi.cn

[R08] 数值比较
来源：http://znn.pycfn.com

if (( a > b )); then echo "a 更大"; fi
来源：http://dbu.bbcook.cn

[R09] 字符串比较
来源：http://fsv.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sdu.gzhubu.top

[R10] 正则匹配
来源：http://fbf.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mgp.zdqjudy.top

[R11] case 多分支
来源：http://umu.yueranfly.top

case "$1" in
来源：http://qtp.hysaishi.cn

start) echo "启动" ;;
来源：http://don.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://pey.yj20258888.top

*)     echo "未知命令" ;;
来源：http://mhw.c1oappe.top

esac
来源：http://psx.ehwqpu.com

[R12] for 遍历文件
来源：http://txa.ydjk.org.cn

for f in *.txt; do echo "$f"; done
来源：http://oby.tarul.cn

[R13] for 计数循环
来源：http://vba.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://jwt.fehbvm.com

[R14] C 风格 for
来源：http://jrs.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sqw.daxiang520.top

[R15] while 逐行读文件
来源：http://eiu.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pxl.jinqigfzy.top

[R16] until 等待条件
来源：http://yxi.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mgu.yanxiufei.cn

[R17] 数组定义与取值
来源：http://ybr.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://qqw.xinyue.icu

[R18] 遍历数组
来源：http://okn.jinqigufen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://taw.zhengqikj.top

[R19] 数组长度
来源：http://axd.hywenlv.cn

echo "${#arr[@]}"
来源：http://auw.xinyue.icu

[R20] 关联数组（字典）
来源：http://qda.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zki.guowangkeji.top

[R21] 字符串长度
来源：http://qdv.hcnkem.com

echo "${#s}"
来源：http://kma.hammf.cn

[R22] 截取子串
来源：http://fnv.xylfe.cn

echo "${s:0:5}"
来源：http://omp.aizwys.cn

[R23] 字符串替换
来源：http://akk.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://loc.zhongyouzk.top

[R24] 大小写转换
来源：http://cdl.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pgj.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://adl.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ood.shanyushiyangtech.top

[R26] 命令替换
来源：http://ulm.sysykeji.top

now=$(date +%F); echo "$now"
来源：http://sov.guannengcc.top

[R27] 算术展开
来源：http://gog.cucudq.cn

echo $((1 + 2 * 3))
来源：http://sxd.svipenyu.cn

[R28] 浮点运算
来源：http://fqz.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://bsw.nwbrower.top

[R29] 定义函数
来源：http://jln.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tkb.jinqigufen.top

[R30] 函数返回状态码
来源：http://ehz.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://rni.tanke756.top

[R31] 局部变量
来源：http://osv.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://bnm.gaohongyu789.top

[R32] 参数个数校验
来源：http://ydt.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fdc.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://fnd.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://swg.nwbrower.top

[R34] 退出时清理
来源：http://bmg.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://irj.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://nlp.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://yjt.dashuyun.cn

[R36] 并发执行多个任务
来源：http://nxi.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dtv.mhx1999.top

[R37] 把输出赋给变量
来源：http://rzh.pycfn.com

files=$(ls -1)
来源：http://eer.aizwys.cn

[R38] 管道串联
来源：http://ufy.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://nif.snrcjt.cn

[R39] 重定向标准输出与错误
来源：http://igm.hfpthk.cn

cmd > out.log 2>&1
来源：http://fen.quarkkingdee.top

[R40] 追加写日志
来源：http://hac.kuanghao11.cn

echo "log" >> out.log
来源：http://zpy.gzhubu.top

[R41] 丢弃输出
来源：http://olz.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://nia.zhongyouzk.top

[R42] 输入重定向
来源：http://eiq.hongshengwenyu.top

wc -l < a.txt
来源：http://vmc.dashuyun.cn

[R43] 按名字查找文件
来源：http://mfs.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://avm.guowangkeji.top

[R44] 按修改时间查找
来源：http://lwm.yanxiufei.cn

find . -mtime -7 -type f
来源：http://lfw.dashuyun.cn

[R45] 批量删除
来源：http://jui.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://lnz.hcnkem.com

[R46] 递归替换文件内容
来源：http://qqj.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://puj.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://mxp.tarul.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qqn.yonumen.top

[R48] awk 取指定列
来源：http://jzw.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://sci.zhiwuduotai.top

[R49] awk 带条件
来源：http://xuq.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://htk.sjlbkw.cn

[R50] awk 求和
来源：http://zfl.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://adr.ctjpmb.com

[R51] 排序去重取前几
来源：http://erv.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vsk.jinyuanbaomall.cn

[R52] 统计行数
来源：http://utt.jinghuilouyu.cn

wc -l a.txt
来源：http://djl.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://sok.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hme.bjfxy.top

[R54] 比较两个文件
来源：http://gqh.quarkkingdee.top

diff a.txt b.txt
来源：http://xnk.zhoulong.xyz

[R55] 压缩与解压
来源：http://yku.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qko.xuetiantiany.cn

[R56] 远程拷贝
来源：http://cjp.yj20258.top

scp file user@host:/path/
来源：http://nll.zhijiandao.cn

[R57] 远程执行命令
来源：http://yft.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://bhp.pycfn.com

[R58] 下载文件
来源：http://yog.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://glo.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://lbk.dianchejie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rbm.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://kwp.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eay.ctjpmb.com

[R61] 磁盘占用
来源：http://jax.shangyingyoupin.top

df -h;  du -sh *
来源：http://ddg.yonumen.top

[R62] 找最占空间的文件
来源：http://frz.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://hbq.cucudq.cn

[R63] 内存与进程
来源：http://nhz.andypj.xyz

free -h;  ps aux | grep nginx
来源：http://hzr.ivvv.top

[R64] 结束进程
来源：http://lpq.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://nlk.yfazqb.com

[R65] 查看端口占用
来源：http://hsj.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cvc.yfazqb.com

[R66] 定时任务
来源：http://rxl.smart0.xyz

crontab -e;  crontab -l
来源：http://pgu.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://ilp.sxryk.cn

openssl rand -hex 16
来源：http://eda.yanxiufei.cn

[R68] 计算文件校验值
来源：http://nip.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pjj.pengpengdd.cyou

[R69] 生成随机密码
来源：http://dki.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://xgb.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://nsr.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://qvd.sjlbkw.cn

[R71] 日期格式化
来源：http://qim.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hrk.meibo888.top

[R72] 等待端口就绪
来源：http://oam.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bvl.ydzc1.top

[R73] 分割大日志
来源：http://snh.ydjk.org.cn

split -l 1000 big.log part_
来源：http://krd.fktsv.cn

[R74] 批量重命名
来源：http://wfv.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cso.hammf.cn

[R75] 导出环境变量
来源：http://cdd.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://rlv.nwbrower.top

[R76] 使用临时文件
来源：http://cpa.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vdl.chenzaomai.com

[R77] 读取用户输入
来源：http://gjz.smart0.xyz

read -rp "请输入: " ans
来源：http://xfz.gaohongyu789.top

[R78] 交互式菜单
来源：http://jyh.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gzv.jinqigufen.top

[R79] 解析命令行选项
来源：http://vrt.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jhy.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://oyp.9152youxi.cn

time ./run.sh
来源：http://bab.hysaishi.cn

================================================================================
来源：http://pfw.vehdjk.com

S. C / C++ 专题
来源：http://lqi.yuxming.cn

================================================================================
来源：http://nwu.havefunace.top

[S01] C：Hello World
来源：http://dij.dianchejie.cn

#include <stdio.h>
来源：http://ipi.shanyushiyangtech.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qlo.yj202588.top

[S02] C：变量与格式化输出
来源：http://xvp.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://iun.316326.xyz

[S03] C：读入整数
来源：http://fqp.andypj.xyz

int x; scanf("%d", &x);
来源：http://oaf.sxryk.cn

[S04] C：字符串复制
来源：http://viw.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nfk.quarkkingdee.top

[S05] C：字符串长度
来源：http://xev.daxiang520.top

strlen(s)
来源：http://tbt.cqqwz.cn

[S06] C：字符串比较
来源：http://wjm.yongpay.top

strcmp(a, b) == 0
来源：http://esa.yongpay.top

[S07] C：数组遍历求和
来源：http://mtd.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vjq.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://xzc.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uml.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://bzj.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://flt.52xcode.cn

[S10] C：指针与解引用
来源：http://khd.52xcode.cn

int *p = &a;  *p = 5;
来源：http://tey.jqgfzy.top

[S11] C：逐行读文件
来源：http://mkm.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://grl.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://drj.chenzaomai.com

fclose(f);
来源：http://uil.iojbl.cn

[S12] C：写文件
来源：http://bdu.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dla.vqdsnc.cn

[S13] C：宏定义
来源：http://xzz.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dzq.chenjidiqi.icu

[S14] C：枚举
来源：http://wfq.yangfankeji.com

enum Color { RED, GREEN, BLUE };
来源：http://znx.shzxlz.cn

[S15] C：类型转换
来源：http://aux.hywenlv.cn

(double) a / b
来源：http://otx.ivvv.top

[S16] C：位操作置位
来源：http://ezt.ybcxt.top

x |= (1 << 3);
来源：http://npv.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://azq.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xes.ydzc1.top

[S18] C：命令行参数
来源：http://uqh.yueranfly.top

int main(int argc, char **argv)
来源：http://rrd.hammf.cn

[S19] C：快速排序
来源：http://oim.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://try.jinqigufen.top

[S20] C：二分查找
来源：http://ivw.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dyq.zycfv.cn

[S21] C：字符类别判断
来源：http://aim.pengpengdd.cyou

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tie.yuxming.cn

[S22] C：字符串转数字
来源：http://oqy.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://vyz.xziqi.cn

[S23] C：随机数
来源：http://jkg.cucudq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nre.cqqwz.cn

[S24] C：获取本地时间
来源：http://xuf.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dve.316326.xyz

[S25] C：内存拷贝
来源：http://egs.yanxiufei.cn

memcpy(dst, src, n);
来源：http://nke.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://jxb.xziqi.cn

memset(a, 0, sizeof a);
来源：http://xti.zhoulong.xyz

[S27] C：定义常量
来源：http://idm.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://aga.sxryk.cn

[S28] C：静态变量
来源：http://gel.tianlin.xyz

static int counter = 0;
来源：http://gdn.daria6918.cn

[S29] C：变参函数
来源：http://lmk.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zfa.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://eio.hnqzz.top

#ifndef X_H
来源：http://mmq.tianlin.xyz

#define X_H
来源：http://eyk.xziqi.cn

#endif
来源：http://qzc.xuanzx.com

[S31] C++：Hello World
来源：http://nqj.pengpengdd.cyou


<!-- 参考信息 -->